# OpenSpace v0.22.1 FP64 Emulation Patches

This directory contains patch files and assets to enable **Dekker/Veltkamp FP64 double-precision emulation** in OpenSpace on modern master (commit `6ea7083177` and compatible commits).

---

## Overview

Many modern graphics processors (such as Intel integrated GPUs, mobile/laptop GPUs, and Apple Silicon under virtualization) have limited or non-existent hardware support for 64-bit floating-point (`double`, `dmat4`, `dvec3`) uniforms and arithmetic in OpenGL shaders.

This patch series adds a runtime-switchable emulation layer:
- **`NO_GPU_DOUBLE=1`**: OpenSpace detects the environment variable and uses emulated single-precision (`..._float.glsl`) shaders, splitting 64-bit transformations and positions into high- and low-order 32-bit floats (`hi`, `lo`) evaluated with Dekker/Veltkamp arithmetic (`shaders/df64.glsl`).
- **`NO_GPU_DOUBLE=0` or unset**: OpenSpace behaves identically to standard upstream OpenSpace, using hardware double-precision uniforms and shaders.

---

## Directory Contents

| File | Purpose |
|---|---|
| `openspace-v0.22.1-fp64-emulation-all.patch` | **Complete unified patch** containing all 98 modified and newly added files. |
| `0001-fp64-emulation-new-shaders-and-headers.patch` | Part 1: All 37 newly added files (`nogpudouble.h`, `df64.glsl`, 35 `..._float.glsl` shaders, and `run_linux.py`). |
| `0002-fp64-emulation-cpp-and-cmake.patch` | Part 2: C++ uniform-splitting logic and CMakeLists registration across 61 files. |
| `openspace-fp64-new-files.tar.gz` | Tar archive of the 37 new files. Extracting this bypasses any line-ending (CRLF vs LF) or whitespace differences when creating new files. |
| `README.md` | This instruction document. |

---

## Patch Application Instructions

### Option A: Single Unified Patch (Recommended)

From the root directory of your cloned OpenSpace repository:

```bash
git apply --ignore-whitespace --ignore-space-change /path/to/openspace-v0.22.1-fp64-emulation-all.patch
```

To test without making changes:
```bash
git apply --check --ignore-whitespace --ignore-space-change /path/to/openspace-v0.22.1-fp64-emulation-all.patch
```

### Option B: Modular Patches (Step-by-Step)

```bash
# 1. Apply new shaders, helper headers, and runner script
git apply --ignore-whitespace --ignore-space-change /path/to/0001-fp64-emulation-new-shaders-and-headers.patch

# 2. Apply C++ uniform splitting and CMake modifications
git apply --ignore-whitespace --ignore-space-change /path/to/0002-fp64-emulation-cpp-and-cmake.patch
```

### Option C: Tarball + C++ Patch (Most Robust on Windows / CI)

On platforms where line endings (CRLF vs LF) might cause issues with `git apply` creating new files:

```bash
# Extract the new files directly
tar -xzf /path/to/openspace-fp64-new-files.tar.gz

# Apply the C++ and CMake modifications
git apply --ignore-whitespace --ignore-space-change /path/to/0002-fp64-emulation-cpp-and-cmake.patch
```

---

## Changes Included in These Patches

1. **`include/openspace/util/nogpudouble.h`**:
   - Central utility providing `nogpudouble::shouldUseDouble()`, checking the `NO_GPU_DOUBLE` environment variable once at startup.
   - Matrix and vector splitting utilities (`splitDmat4`, `splitDvec3`, `splitDvec4`) using Dekker/Veltkamp two-sum arithmetic.

2. **`shaders/df64.glsl`**:
   - GLSL library implementing Dekker/Veltkamp double-precision emulation in single-precision floats: `df64_add`, `df64_sub`, `df64_mul`, `df64_vec3_sub`, `df64_mat4_mul_vec4`, etc.

3. **Modules Updated**:
   - `atmosphere`: Atmosphere deferred raycaster with split view-to-object and model transforms, light-time shadow offset, and altitude clamping.
   - `base`: Grids (box, planar, radial, spherical), point clouds (Tully galaxies fix with view-space scaling), trails, models, arrows, and lines.
   - `digitaluniverse`: DU mesh rendering.
   - `fieldlinessequence`: Fieldlines rendering.
   - `gaia`: Gaia star rendering and tonemapping.
   - `galaxy`: Galaxy raycasting, billboards, and bounds.
   - `globebrowsing`: Global/local patch rendering, GeoJSON billboards, ring systems, and relative-position eclipse shadows.
   - `solarbrowsing`: Spacecraft image projection.
   - `space`: Constellation lines, flux nodes, orbital Kepler trails & points, star billboards, and travel speed.

4. **Visual Testing Suite (`support/runner/run_linux.py`)**:
   - Customized Linux test runner supporting `openspace` CLI wrapper.
   - `-a` (attach/poll) mode with snapshotting to prevent overwriting screenshots.
   - Dry-run mode (`--dry-run`) for warming caches across all visual tests without rendering overhead.

---

## GitHub Actions CI Workflow Example

Here is a ready-to-use GitHub Actions workflow to build and test OpenSpace with these patches:

```yaml
name: Build OpenSpace with FP64 Emulation

on:
  push:
    branches: [ master, main ]
  pull_request:

jobs:
  build:
    name: Build (${{ matrix.os }})
    runs-on: ${{ matrix.os }}
    strategy:
      fail-fast: false
      matrix:
        os: [ubuntu-24.04, windows-2022]

    steps:
      - name: Checkout OpenSpace Master
        uses: actions/checkout@v4
        with:
          repository: OpenSpace/OpenSpace
          ref: master
          submodules: recursive
          path: openspace

      - name: Checkout Patches
        uses: actions/checkout@v4
        with:
          path: patches

      - name: Apply FP64 Emulation Patches (Linux)
        if: runner.os == 'Linux'
        working-directory: openspace
        run: |
          git apply --ignore-whitespace --ignore-space-change ../patches/v0-22-1-patches/openspace-v0.22.1-fp64-emulation-all.patch
          git status -s

      - name: Apply FP64 Emulation Patches (Windows)
        if: runner.os == 'Windows'
        working-directory: openspace
        shell: bash
        run: |
          tar -xzf ../patches/v0-22-1-patches/openspace-fp64-new-files.tar.gz
          git apply --ignore-whitespace --ignore-space-change ../patches/v0-22-1-patches/0002-fp64-emulation-cpp-and-cmake.patch
          git status -s

      - name: Setup Dependencies (Linux)
        if: runner.os == 'Linux'
        run: |
          sudo apt-get update
          sudo apt-get install -y ninja-build cmake libgl1-mesa-dev libglu1-mesa-dev \
            libxrandr-dev libxinerama-dev libxcursor-dev libxi-dev libasound2-dev

      - name: Configure CMake
        working-directory: openspace
        run: |
          cmake -B build -G "Ninja" \
            -DCMAKE_BUILD_TYPE=Release \
            -DOPENSPACE_WARNINGS_AS_ERRORS=OFF

      - name: Build OpenSpace
        working-directory: openspace
        run: |
          cmake --build build --config Release --parallel

      - name: Test Running in FP64 Emulation Mode (Linux Headless)
        if: runner.os == 'Linux'
        working-directory: openspace
        run: |
          sudo apt-get install -y xvfb
          xvfb-run -a env NO_GPU_DOUBLE=1 ./bin/OpenSpace --help || true
```

---

## Verifying Runtime Execution

After building OpenSpace, you can verify both paths:

```bash
# 1. Native Double Path (baseline)
./bin/OpenSpace

# 2. FP64 Emulated Float Path
```
On Linux and Mac,
```
export NO_GPU_DOUBLE=1 
./bin/OpenSpace
```
On Windows Powershell,
```
$env.NO_GPU_DOUBLE=1
bin/OpenSpace
```
On Windows `cmd`,
```
set NO_GPU_DOUBLE=1
bin/OpenSpace
```

Check the log or console output:
- In `NO_GPU_DOUBLE=1` mode, shaders such as `atmosphere_deferred_fs_float.glsl` and `pointcloud_gs_float.glsl` will be loaded, and hardware double requirements are bypassed.
