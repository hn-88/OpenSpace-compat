# Conversation Prompts and Execution History

This document records every user prompt submitted in this thread and project, the model used to produce the reply, and the total duration the agent took to work out each response.

## Summary Table

| # | Model | Duration | Timestamp (UTC) | Prompt Summary |
|---|---|---|---|---|
| 1 | Claude Sonnet 4.6 (Thinking) | 10m 54s | 2026-10-16T08:02:46Z | The atmosphere module of OpenSpace, at https://github.com/OpenSpace/Open... |
| 2 | Claude Sonnet 4.6 (Thinking) | 9m 41s | 2026-10-16T08:20:10Z | Please rewrite the module using the practical fixes and the flowchart yo... |
| 3 | Claude Sonnet 4.6 (Thinking) | 9m 22s | 2026-10-17T03:47:46Z | Please continue this task in case you have not finished. |
| 4 | Claude Sonnet 4.6 (Thinking) | 45s | 2026-10-18T04:04:18Z | A couple of problems noticed after building on Github runner and running... |
| 5 | Gemini 3.8 Flash (Medium) | 0s | 2026-10-18T04:09:25Z | Can I change the model to Gemini 3.8 Flash and continue working on this ... |
| 6 | Gemini 3.8 Flash (Medium) | 4m 18s | 2026-10-18T04:09:49Z | Yes |
| 7 | Gemini 3.8 Flash (Medium) | 2m 52s | 2026-10-18T04:17:33Z | Please don't do this - "Detect capability at startup with GL_ARB_gpu_sha... |
| 8 | Gemini 3.8 Flash (Medium) | 0s | 2026-10-18T08:02:57Z | Can you please show me the lines where the C++ caster will  load the com... |
| 9 | Gemini 3.8 Flash (Medium) | 5s | 2026-10-18T08:04:38Z | OK. Please give me a list of files which have been modified in the OpenS... |
| 10 | Gemini 3.8 Flash (Medium) | 6m 44s | 2026-10-19T03:14:26Z | This version of the atmosphere double workaround compiles and runs. But,... |
| 11 | Gemini 3.8 Flash (Medium) | 17m 44s | 2026-10-20T03:19:48Z | This version compiles and runs. But the atmosphere shading in the NO_GPU... |
| 12 | Gemini 3.8 Flash (Medium) | 16m 52s | 2026-10-20T05:32:21Z | This version is much improved, thank you. But still, there are differenc... |
| 13 | Gemini 3.8 Flash (Medium) | 13m 26s | 2026-10-20T07:25:42Z | Can you please construct shaders with the float workaround without losin... |
| 14 | Gemini 3.8 Flash (Medium) | 8m 17s | 2026-10-20T07:45:11Z | Can you please verify that the float.glsl shaders give the same output a... |
| 15 | Gemini 3.8 Flash (Medium) | 6m 15s | 2026-10-21T03:38:30Z | Unfortunately, the OpenSpace codebase in the project directory seems to ... |
| 16 | Gemini 3.8 Flash (Medium) | 4m 59s | 2026-10-21T05:56:29Z | After building and running this, I see this behaviour. With the original... |
| 17 | Gemini 3.8 Flash (Medium) | 9s | 2026-10-21T08:18:12Z | OK, I have tested and everything seems fine. Once again, please give me ... |
| 18 | Gemini 3.8 Flash (Medium) | 56m 48s | 2026-10-24T03:30:44Z | All right. These are tested and working. Now, please go through the enti... |
| 19 | Gemini 3.8 Flash (Medium) | 2m 34s | 2026-10-24T05:16:47Z | OK, let me build and test this. Meanwhile, I see that OpenSpace has a vi... |
| 20 | Gemini 3.8 Flash (Medium) | 4m 22s | 2026-10-24T07:30:40Z | Build failed. Here are the last few lines of the build workflow logs.  [... |
| 21 | Gemini 3.8 Flash (Medium) | 3m 3s | 2026-10-24T08:06:37Z | Another build error, logs below.  [338/1045] Building CXX object modules... |
| 22 | Gemini 3.8 Flash (Medium) | 1m 49s | 2026-10-24T08:52:13Z | Further build error,  [446/1045] Building CXX object modules/galaxy/CMak... |
| 23 | Gemini 3.8 Flash (Medium) | 2m 53s | 2026-10-25T03:14:04Z | Next build error -   [460/1045] Building CXX object modules/globebrowsin... |
| 24 | Gemini 3.8 Flash (Medium) | 1m 26s | 2026-10-25T03:55:30Z | Next build error,  [587/1045] Building CXX object modules/space/CMakeFil... |
| 25 | Gemini 3.8 Flash (Medium) | 9m 12s | 2026-10-29T03:51:13Z | When this is built and tested on Windows, we get errors like this,  Coul... |
| 26 | Gemini 3.8 Flash (Medium) | 2m 58s | 2026-10-29T04:18:54Z | Then, how about deleting the extra unnecessary copies of df64.glsl, sinc... |
| 27 | Gemini 3.8 Flash (Medium) | 4m 42s | 2026-10-29T04:23:37Z | Can you now check that all these errors have been resolved with the curr... |
| 28 | Gemini 3.8 Flash (Medium) | 21s | 2026-10-29T04:37:05Z | Please list the paths to all the files deleted and all the files added o... |
| 29 | Gemini 3.8 Flash (Medium) | 3m 2s | 2026-10-30T03:35:43Z | Now I get errors like this. Please check how the other shaders in OpenSp... |
| 30 | Gemini 3.8 Flash (Medium) | 1m 40s | 2026-10-30T07:37:26Z | After fixing that, now the errors are:  2026-10-30	12:37:57.206	OpenGL (... |
| 31 | Gemini 3.8 Flash (Medium) | 6m 50s | 2026-10-31T03:14:50Z | Now those errors are gone. OpenSpace does run. But the renderabletrails ... |
| 32 | Gemini 3.8 Flash (Medium) | 9m 46s | 2026-10-31T03:29:32Z | Can you check all the "renderable" files for such inconsistencies betwee... |
| 33 | Gemini 3.8 Flash (Medium) | 10m 32s | 2026-11-01T08:31:28Z | I'm trying to test OpenSpace running with Dekker Veltkamp fp64 emulation... |
| 34 | Gemini 3.8 Flash (Medium) | 7m 34s | 2026-11-02T07:38:54Z | The "Tully Galaxy Images" are rendering fine on Windows+Intel and Linux+... |
| 35 | Gemini 3.8 Flash (Medium) | 5m 11s | 2026-11-02T08:11:52Z | This seems to have fixed the problem, thank you. Now I would like to run... |
| 36 | Gemini 3.8 Flash (Medium) | 3m 11s | 2026-11-02T08:52:15Z | In -a mode, when we run multiple tests, the copy command is copying all ... |
| 37 | Gemini 3.8 Flash (Medium) | 0s | 2026-11-02T08:57:02Z | Would not a simple replacement of the copy command with a move command i... |
| 38 | Gemini 3.8 Flash (Medium) | 10m 59s | 2026-11-03T03:36:41Z | Now, the fp64 emulation works well. But the OpenSpace master branch has ... |
| 39 | Gemini 3.8 Flash (Medium) | 14m 52s | 2026-11-04T04:49:07Z | Doing visual regression tests between the NO_GPU_DOUBLE=1 and NO_GPU_DOU... |
| 40 | Gemini 3.8 Flash (Medium) | Current turn (generating Prompts.md) | 2026-11-05T03:25:49Z | Can you make a single document called Prompts.md which lists 1. Every si... |

---

## Detailed Prompts

### Prompt 1
- **Model Used**: Claude Sonnet 4.6 (Thinking)
- **Start Time (UTC)**: `2026-10-16T08:02:46Z`
- **Completion Time (UTC)**: `2026-10-16T08:13:40Z`
- **Response Duration**: **10m 54s**

**Prompt:**
```text
The atmosphere module of OpenSpace, at
https://github.com/OpenSpace/OpenSpace/tree/master/modules/atmosphere
is one of the OpenSpace modules that makes extensive use of double uniforms and GPU calculations on double values. This module slows down rendering a lot by failing over to CPU, when some devices have GPU drivers and or hardware that don't support double data types. Can you look at the code and think of some workarounds so that the "double" calculations can be done by GPU float types without loss of data? Perhaps by using two floats for each double or something like that?
```

### Prompt 2
- **Model Used**: Claude Sonnet 4.6 (Thinking)
- **Start Time (UTC)**: `2026-10-16T08:20:10Z`
- **Completion Time (UTC)**: `2026-10-16T08:29:51Z`
- **Response Duration**: **9m 41s**

**Prompt:**
```text
Please rewrite the module using the practical fixes and the flowchart you have suggested.
```

### Prompt 3
- **Model Used**: Claude Sonnet 4.6 (Thinking)
- **Start Time (UTC)**: `2026-10-17T03:47:46Z`
- **Completion Time (UTC)**: `2026-10-17T03:57:08Z`
- **Response Duration**: **9m 22s**

**Prompt:**
```text
Please continue this task in case you have not finished.
```

### Prompt 4
- **Model Used**: Claude Sonnet 4.6 (Thinking)
- **Start Time (UTC)**: `2026-10-18T04:04:18Z`
- **Completion Time (UTC)**: `2026-10-18T04:05:03Z`
- **Response Duration**: **45s**

**Prompt:**
```text
A couple of problems noticed after building on Github runner and running on a Windows machine with Intel graphics - though the graphics becomes quite slow if atmosphere is enabled, the system capabilities still lists fp64 as available. Probably the driver emulates it in CPU. So, instead of relying on run-time detection, we can modify the code to look for an environment variable which we could set on Windows before running OpenSpace like
set NO_DOUBLE=1 && OpenSpace
or something like that.

The second problem seems to be that the shader files go through all the branches when being sent to the driver for interpretation. So, we need to have two separate shader files, one for the double workaround and one without the double workaround, to avoid errors - the loading of the shaders should of course be based on the environment variable set as above.

You can see the errors below, and see if any other changes would need to be made.

026-10-17 | 17:38:30.957 | OpenGL (Shader Compiler) [Error] {0} | Error | SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 338, "Deferred 0 raycast Fragment": ERROR: 0:829: 'normalWorldSpace' : redefinitionERROR: 0:860: 'inscatterRadiance' : no matching overloaded function found (using implicit conversion)ERROR: 0:860: 'inscatterRadiance' : function is not knownERROR: 0:857: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
-- | -- | -- | -- | --
2026-10-17 | 17:38:31.327 | OpenGL (Shader Compiler) [Error] {0} | Debug | Stacktrace0: OpenSpace+0x877F7B1: OpenSpace+0x8482052: OpenSpace+0xAA20733: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B6545: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB236: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F7: OpenSpace+0xCB07088: OpenSpace+0xBD24CF9: OpenSpace+0xBD04A510: OpenSpace+0xBE50F911: OpenSpace+0xBE47C512: OpenSpace+0x89363113: OpenSpace+0x7E75E514: OpenSpace+0xD610D615: OpenSpace+0x7EBB4616: OpenSpace!NCJunparse+0x1E6C42C17: KERNEL32!BaseThreadInitThunk+0x1718: ntdll!RtlUserThreadStart+0x2C
2026-10-17 | 17:38:31.333 | ShaderObject | Error | Error compiling shader object [Deferred 0 raycast Fragment]: ERROR: 0:829: 'normalWorldSpace' : redefinitionERROR: 0:860: 'inscatterRadiance' : no matching overloaded function found (using implicit conversion)ERROR: 0:860: 'inscatterRadiance' : function is not knownERROR: 0:857: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'0: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\atmosphere_deferred_fs.glsl1: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\df64.glsl2: D:\Downloads\OpenSpace-minimal-test-vcpkg\shaders\floatoperations.glsl3: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\atmosphere_common.glsl
2026-10-17 | 17:38:31.342 | OpenGL (Shader Compiler) [Error] {0} | Error | SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 338, "Deferred 1 raycast Fragment": ERROR: 0:829: 'normalWorldSpace' : redefinitionERROR: 0:860: 'inscatterRadiance' : no matching overloaded function found (using implicit conversion)ERROR: 0:860: 'inscatterRadiance' : function is not knownERROR: 0:857: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
2026-10-17 | 17:38:31.342 | OpenGL (Shader Compiler) [Error] {0} | Debug | Stacktrace0: OpenSpace+0x877F7B1: OpenSpace+0x8482052: OpenSpace+0xAA20733: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B6545: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB236: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F7: OpenSpace+0xCB07088: OpenSpace+0xBD24CF9: OpenSpace+0xBD04A510: OpenSpace+0xBE50F911: OpenSpace+0xBE47C512: OpenSpace+0x89363113: OpenSpace+0x7E75E514: OpenSpace+0xD610D615: OpenSpace+0x7EBB4616: OpenSpace!NCJunparse+0x1E6C42C17: KERNEL32!BaseThreadInitThunk+0x1718: ntdll!RtlUserThreadStart+0x2C
2026-10-17 | 17:38:31.342 | ShaderObject | Error | Error compiling shader object [Deferred 1 raycast Fragment]: ERROR: 0:829: 'normalWorldSpace' : redefinitionERROR: 0:860: 'inscatterRadiance' : no matching overloaded function found (using implicit conversion)ERROR: 0:860: 'inscatterRadiance' : function is not knownERROR: 0:857: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'0: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\atmosphere_deferred_fs.glsl1: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\df64.glsl2: D:\Downloads\OpenSpace-minimal-test-vcpkg\shaders\floatoperations.glsl3: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\atmosphere_common.glsl
2026-10-17 | 17:38:31.349 | OpenGL (Shader Compiler) [Error] {0} | Error | SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 338, "Deferred 2 raycast Fragment": ERROR: 0:829: 'normalWorldSpace' : redefinitionERROR: 0:860: 'inscatterRadiance' : no matching overloaded function found (using implicit conversion)ERROR: 0:860: 'inscatterRadiance' : function is not knownERROR: 0:857: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
2026-10-17 | 17:38:31.349 | OpenGL (Shader Compiler) [Error] {0} | Debug | Stacktrace0: OpenSpace+0x877F7B1: OpenSpace+0x8482052: OpenSpace+0xAA20733: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B6545: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB236: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F7: OpenSpace+0xCB07088: OpenSpace+0xBD24CF9: OpenSpace+0xBD04A510: OpenSpace+0xBE50F911: OpenSpace+0xBE47C512: OpenSpace+0x89363113: OpenSpace+0x7E75E514: OpenSpace+0xD610D615: OpenSpace+0x7EBB4616: OpenSpace!NCJunparse+0x1E6C42C17: KERNEL32!BaseThreadInitThunk+0x1718: ntdll!RtlUserThreadStart+0x2C
2026-10-17 | 17:38:31.349 | ShaderObject | Error | Error compiling shader object [Deferred 2 raycast Fragment]: ERROR: 0:829: 'normalWorldSpace' : redefinitionERROR: 0:860: 'inscatterRadiance' : no matching overloaded function found (using implicit conversion)ERROR: 0:860: 'inscatterRadiance' : function is not knownERROR: 0:857: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'0: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\atmosphere_deferred_fs.glsl1: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\df64.glsl2: D:\Downloads\OpenSpace-minimal-test-vcpkg\shaders\floatoperations.glsl3: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\atmosphere_common.glsl
2026-10-17 | 17:38:31.349 | OpenGL (Shader Compiler) [Error] {0} | Error | SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 338, "Deferred 3 raycast Fragment": ERROR: 0:829: 'normalWorldSpace' : redefinitionERROR: 0:860: 'inscatterRadiance' : no matching overloaded function found (using implicit conversion)ERROR: 0:860: 'inscatterRadiance' : function is not knownERROR: 0:857: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
2026-10-17 | 17:38:31.349 | OpenGL (Shader Compiler) [Error] {0} | Debug | Stacktrace0: OpenSpace+0x877F7B1: OpenSpace+0x8482052: OpenSpace+0xAA20733: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B6545: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB236: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F7: OpenSpace+0xCB07088: OpenSpace+0xBD24CF9: OpenSpace+0xBD04A510: OpenSpace+0xBE50F911: OpenSpace+0xBE47C512: OpenSpace+0x89363113: OpenSpace+0x7E75E514: OpenSpace+0xD610D615: OpenSpace+0x7EBB4616: OpenSpace!NCJunparse+0x1E6C42C17: KERNEL32!BaseThreadInitThunk+0x1718: ntdll!RtlUserThreadStart+0x2C
2026-10-17 | 17:38:31.349 | ShaderObject | Error | Error compiling shader object [Deferred 3 raycast Fragment]: ERROR: 0:829: 'normalWorldSpace' : redefinitionERROR: 0:860: 'inscatterRadiance' : no matching overloaded function found (using implicit conversion)ERROR: 0:860: 'inscatterRadiance' : function is not knownERROR: 0:857: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'0: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\atmosphere_deferred_fs.glsl1: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\df64.glsl2: D:\Downloads\OpenSpace-minimal-test-vcpkg\shaders\floatoperations.glsl3: D:\Downloads\OpenSpace-minimal-test-vcpkg\modules\atmosphere\shaders\atmosphere_common.glsl
2026-10-17 | 17:38:31.357 | Logging | Warning | Number of Errors: 8
2026-10-17 | 17:38:32.570 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.570 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.570 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.570 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.329 | PathNavigator | Debug | The scene graph node 'Root' has no, or a very small, bounding sphere. Using minimal value of 10. This might lead to unexpected results
2026-10-17 | 17:38:32.329 | PathNavigator | Debug | The scene graph node 'Root' has no, or a very small, bounding sphere. Using minimal value of 10. This might lead to unexpected results
2026-10-17 | 17:38:32.329 | PathNavigator | Debug | Successfully generated camera path
2026-10-17 | 17:38:32.329 | OpenSpaceEngine | Debug | Mode: CameraPath
2026-10-17 | 17:38:32.329 | PathNavigator | Info | Pausing time simulation during path traversal
2026-10-17 | 17:38:32.329 | PathNavigator | Info | Starting path
2026-10-17 | 17:38:32.336 | Logging | Warning | Number of Warnings: 4
2026-10-17 | 17:38:32.338 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.341 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.341 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.341 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.345 | PathNavigator | Info | Reached target
2026-10-17 | 17:38:32.345 | OpenSpaceEngine | Debug | Reset engine mode to 'UserControl'
2026-10-17 | 17:38:32.373 | Logging | Warning | Number of Warnings: 4
2026-10-17 | 17:38:32.685 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.687 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
2026-10-17 | 17:38:32.687 | FramebufferRenderer | Warning | Deferredcaster is not attached when trying to perform deferred task
```

### Prompt 5
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-18T04:09:25Z`
- **Completion Time (UTC)**: `2026-10-18T04:09:25Z`
- **Response Duration**: **0s**

**Prompt:**
```text
Can I change the model to Gemini 3.8 Flash and continue working on this thread? Even though the Claude quota is reached?
```

### Prompt 6
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-18T04:09:49Z`
- **Completion Time (UTC)**: `2026-10-18T04:14:07Z`
- **Response Duration**: **4m 18s**

**Prompt:**
```text
Yes
```

### Prompt 7
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-18T04:17:33Z`
- **Completion Time (UTC)**: `2026-10-18T04:20:25Z`
- **Response Duration**: **2m 52s**

**Prompt:**
```text
Please don't do this - "Detect capability at startup with GL_ARB_gpu_shader_fp64" - Instead, please get the value of NO_GPU_DOUBLE as an environment variable set on the machine before starting OpenSpace.
```

### Prompt 8
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-18T08:02:57Z`
- **Completion Time (UTC)**: `2026-10-18T08:02:57Z`
- **Response Duration**: **0s**

**Prompt:**
```text
Can you please show me the lines where the C++ caster will  load the companion shader atmosphere_deferred_fs_float.glsl ? Has that been implemented? Let me review it.
```

### Prompt 9
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-18T08:04:38Z`
- **Completion Time (UTC)**: `2026-10-18T08:04:43Z`
- **Response Duration**: **5s**

**Prompt:**
```text
OK. Please give me a list of files which have been modified in the OpenSpace codebase, so that I can drag and drop them into a commit, build and test on my test branch.
```

### Prompt 10
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-19T03:14:26Z`
- **Completion Time (UTC)**: `2026-10-19T03:21:10Z`
- **Response Duration**: **6m 44s**

**Prompt:**
```text
This version of the atmosphere double workaround compiles and runs. But, when using the NO_GPU_DOUBLE override, the atmosphere renders as large blocks of equal colour instead of as a continuously varying spherical blanket around the planet. Perhaps some assumptions used to truncate doubles to floats are not valid. Can you rewrite, perhaps using the Dekker/Veltkamp emulation method for all double calls?
```

### Prompt 11
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-20T03:19:48Z`
- **Completion Time (UTC)**: `2026-10-20T03:37:32Z`
- **Response Duration**: **17m 44s**

**Prompt:**
```text
This version compiles and runs. But the atmosphere shading in the NO_GPU_DOUBLE path is still not the same as in the other path. Instead of a uniformly fading atmosphere, we see triangles, and the atmosphere flashing on and off at certain elevations. Please check whether the shader math gives the same result in the same paths. If yes, then the problem may be in the setting of the uniforms at the CPU C++ code - that also would need a separate path if NO_GPU_DOUBLE .
```

### Prompt 12
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-20T05:32:21Z`
- **Completion Time (UTC)**: `2026-10-20T05:49:13Z`
- **Response Duration**: **16m 52s**

**Prompt:**
```text
This version is much improved, thank you. But still, there are differences between the original double shader and the NO_GPU_DOUBLE path. For example, when moving down towards Earth, the original shader shows the land through the diffuse lighting of the atmosphere throughout, while when using the NO_GPU_DOUBLE path, the atmosphere diffuseness seen on Earth's surface suddenly kicks in at an altitude of around 80-90 km - higher than that altitude, the surface is shaded as if the atmosphere module was turned off.
```

### Prompt 13
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-20T07:25:42Z`
- **Completion Time (UTC)**: `2026-10-20T07:39:08Z`
- **Response Duration**: **13m 26s**

**Prompt:**
```text
Can you please construct shaders with the float workaround without losing precision, for the renderablestars module also, OpenSpace/modules/space/rendering/renderablestars.cpp
```

### Prompt 14
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-20T07:45:11Z`
- **Completion Time (UTC)**: `2026-10-20T07:53:28Z`
- **Response Duration**: **8m 17s**

**Prompt:**
```text
Can you please verify that the float.glsl shaders give the same output as the original glsl files? That there are no extra precision truncations being performed?
```

### Prompt 15
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-21T03:38:30Z`
- **Completion Time (UTC)**: `2026-10-21T03:44:45Z`
- **Response Duration**: **6m 15s**

**Prompt:**
```text
Unfortunately, the OpenSpace codebase in the project directory seems to have regressed. After my prompt "Can you please construct shaders with the float workaround without losing precision, for the renderablestars module also, OpenSpace/modules/space/rendering/renderablestars.cpp"
the code in the codebase does not produce the log line indicating that the environment variable NO_GPU_DOUBLE was detected, and that the ...float.glsl shader is being used. Can you please check what caused this problem? As a reminder, what I want is, if NO_GPU_DOUBLE env var is not set, or is set to 0, the original OpenSpace shaders should be used, while if that variable is set to 1, the float workaround should be used for the renderablestar and atmosphere modules.
```

### Prompt 16
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-21T05:56:29Z`
- **Completion Time (UTC)**: `2026-10-21T06:01:28Z`
- **Response Duration**: **4m 59s**

**Prompt:**
```text
After building and running this, I see this behaviour. With the original shader path, everything is normal, as it should be. With the NO_GPU_DOUBLE path, the Info logging shows that the float glsl files are being used. The Earth atmosphere looks OK - (I have not verified whether it actually uses the float workaround.) But the renderablestars have a problem. The renderable stars load OK, but If we zoom in or out in the scene, the stars start getting bigger and bigger, and finally make the entire screen white.
```

### Prompt 17
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-21T08:18:12Z`
- **Completion Time (UTC)**: `2026-10-21T08:18:21Z`
- **Response Duration**: **9s**

**Prompt:**
```text
OK, I have tested and everything seems fine. Once again, please give me a list of all the files which have changed from the original OpenSpace codebase, so that I can double-check that I have committed all the required files to a new branch.
```

### Prompt 18
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-24T03:30:44Z`
- **Completion Time (UTC)**: `2026-10-24T04:27:32Z`
- **Response Duration**: **56m 48s**

**Prompt:**
```text
All right. These are tested and working. Now, please go through the entire OpenSpace codebase and create such alternate ...float.glsl shaders and supporting Dekker/Veltkamp code for every uniform which uses double (fp64) types. Please follow the same mechanism which you did for atmosphere and renderablestars, viz, please retain the current shaders/uniforms and only use the float uniforms / shaders if the environment variable NO_GPU_DOUBLE is set to 1.
```

### Prompt 19
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-24T05:16:47Z`
- **Completion Time (UTC)**: `2026-10-24T05:19:21Z`
- **Response Duration**: **2m 34s**

**Prompt:**
```text
OK, let me build and test this. Meanwhile, I see that OpenSpace has a visualtests directory. I believe somewhere in github.com/OpenSpace, there may be some documentation on how to run automated tests on OpenSpace. Can you please tell me the details, how I can run automated visual tests with screenshots and differences, running on Linux Mint (OpenSpace's tests might be on Windows) - I would like to test this emulated version versus the original OpenSpace version - that is, with and without the NO_GPU_DOUBLE environment variable.
```

### Prompt 20
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-24T07:30:40Z`
- **Completion Time (UTC)**: `2026-10-24T07:35:02Z`
- **Response Duration**: **4m 22s**

**Prompt:**
```text
Build failed. Here are the last few lines of the build workflow logs.

[315/1045] Building CXX object src/CMakeFiles/openspace-core.dir/util/transformationmanager.cpp.o
[316/1045] Building CXX object src/CMakeFiles/openspace-core.dir/util/universalhelpers.cpp.o
[317/1045] Building CXX object src/CMakeFiles/openspace-core.dir/util/timemanager.cpp.o
[318/1045] Building CXX object src/CMakeFiles/openspace-core.dir/util/versionchecker.cpp.o
[319/1045] Building CXX object modules/base/CMakeFiles/openspace-module-base.dir/basemodule.cpp.o
FAILED: modules/base/CMakeFiles/openspace-module-base.dir/basemodule.cpp.o 
/usr/bin/c++ -DCURL_STATICLIB -DD_GNU_SOURCE -DGLBINDING_AUX_STATIC_DEFINE -DGLBINDING_STATIC_DEFINE -DHAS_STRING_VIEW=1 -DONLY_C_LOCALE=0 -DOPENSPACE_DEBUG -DOPENSPACE_LOGGING_ENABLE_TRACE -DOPENSPACE_MODULE_ATMOSPHERE_ENABLED -DOPENSPACE_MODULE_AUDIO_ENABLED -DOPENSPACE_MODULE_BASE_ENABLED -DOPENSPACE_MODULE_CEFWEBGUI_ENABLED -DOPENSPACE_MODULE_DEBUGGING_ENABLED -DOPENSPACE_MODULE_DIGITALUNIVERSE_ENABLED -DOPENSPACE_MODULE_EXOPLANETS_ENABLED -DOPENSPACE_MODULE_FIELDLINESSEQUENCE_ENABLED -DOPENSPACE_MODULE_FIELDLINES_ENABLED -DOPENSPACE_MODULE_FITSFILEREADER_ENABLED -DOPENSPACE_MODULE_GAIA_ENABLED -DOPENSPACE_MODULE_GALAXY_ENABLED -DOPENSPACE_MODULE_GLOBEBROWSING_ENABLED -DOPENSPACE_MODULE_IMGUI_ENABLED -DOPENSPACE_MODULE_ISWA_ENABLED -DOPENSPACE_MODULE_KAMELEONVOLUME_ENABLED -DOPENSPACE_MODULE_KAMELEON_ENABLED -DOPENSPACE_MODULE_MOLECULE_ENABLED -DOPENSPACE_MODULE_MULTIRESVOLUME_ENABLED -DOPENSPACE_MODULE_OPENSOUNDCONTROL_ENABLED -DOPENSPACE_MODULE_SKYBROWSER_ENABLED -DOPENSPACE_MODULE_SOLARBROWSING_ENABLED -DOPENSPACE_MODULE_SPACECRAFTINSTRUMENTS_ENABLED -DOPENSPACE_MODULE_SPACE_ENABLED -DOPENSPACE_MODULE_STATEMACHINE_ENABLED -DOPENSPACE_MODULE_SYNC_ENABLED -DOPENSPACE_MODULE_TELEMETRY_ENABLED -DOPENSPACE_MODULE_TOUCH_ENABLED -DOPENSPACE_MODULE_VIDEO_ENABLED -DOPENSPACE_MODULE_VOLUME_ENABLED -DOPENSPACE_MODULE_WEBBROWSER_ENABLED -DOPENSPACE_MODULE_WEBGUI_ENABLED -DSYSTEM_LINUX -D_GLIBCXX_USE_TBB_PAR_BACKEND=0 -D_PSTL_PAR_BACKEND_SERIAL -I/workspace -I/workspace/include -I/workspace/build/_generated/include -isystem /vcpkg/installed/x64-linux/include -isystem /workspace/ext/renderdoc -isystem /vcpkg/installed/x64-linux/include/kubazip -O3 -DNDEBUG -std=gnu++23 -ggdb -march=x86-64-v3 -Wall -Wextra -Wpedantic -Walloc-zero -Wcast-qual -Wdate-time -Wduplicated-branches -Wduplicated-cond -Wenum-conversion -Wformat=2 -Wformat-signedness -Wimplicit-fallthrough -Winvalid-utf8 -Wlogical-op -Wmain -Wno-changes-meaning -Wshadow -Wundef -Wunused -Wuninitialized -Wvla -Wzero-as-null-pointer-constant -Wno-attributes -Wno-missing-field-initializers -DSCN_REGEX_BACKEND=0 -Winvalid-pch -include /workspace/build/modules/base/CMakeFiles/openspace-module-base.dir/cmake_pch.hxx -MD -MT modules/base/CMakeFiles/openspace-module-base.dir/basemodule.cpp.o -MF modules/base/CMakeFiles/openspace-module-base.dir/basemodule.cpp.o.d -o modules/base/CMakeFiles/openspace-module-base.dir/basemodule.cpp.o -c /workspace/modules/base/basemodule.cpp
In file included from /workspace/build/modules/base/CMakeFiles/openspace-module-base.dir/cmake_pch.hxx:25,
                 from <command-line>:
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:242:9: error: 'cameraViewMatrix_hi' has not been declared
  242 |         cameraViewMatrix_hi, cameraViewMatrix_lo, projectionMatrix, modelMatrix_hi,
      |         ^~~~~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:242:30: error: 'cameraViewMatrix_lo' has not been declared
  242 |         cameraViewMatrix_hi, cameraViewMatrix_lo, projectionMatrix, modelMatrix_hi,
      |                              ^~~~~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:242:51: error: 'projectionMatrix' has not been declared
  242 |         cameraViewMatrix_hi, cameraViewMatrix_lo, projectionMatrix, modelMatrix_hi,
      |                                                   ^~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:242:69: error: 'modelMatrix_hi' has not been declared
  242 |         cameraViewMatrix_hi, cameraViewMatrix_lo, projectionMatrix, modelMatrix_hi,
      |                                                                     ^~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:243:9: error: 'modelMatrix_lo' has not been declared
  243 |         modelMatrix_lo, cameraPosition_hi, cameraPosition_lo, cameraLookUp,
      |         ^~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:243:25: error: 'cameraPosition_hi' has not been declared
  243 |         modelMatrix_lo, cameraPosition_hi, cameraPosition_lo, cameraLookUp,
      |                         ^~~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:243:44: error: 'cameraPosition_lo' has not been declared
  243 |         modelMatrix_lo, cameraPosition_hi, cameraPosition_lo, cameraLookUp,
      |                                            ^~~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:243:63: error: 'cameraLookUp' has not been declared
  243 |         modelMatrix_lo, cameraPosition_hi, cameraPosition_lo, cameraLookUp,
      |                                                               ^~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:244:9: error: 'renderOption' has not been declared
  244 |         renderOption, maxAngularSize, color, opacity, scaleExponent, scaleFactor, up,
      |         ^~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:244:23: error: 'maxAngularSize' has not been declared
  244 |         renderOption, maxAngularSize, color, opacity, scaleExponent, scaleFactor, up,
      |                       ^~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:244:39: error: 'color' has not been declared
  244 |         renderOption, maxAngularSize, color, opacity, scaleExponent, scaleFactor, up,
      |                                       ^~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:244:46: error: 'opacity' is not a type
  244 |         renderOption, maxAngularSize, color, opacity, scaleExponent, scaleFactor, up,
      |                                              ^~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:244:55: error: 'scaleExponent' has not been declared
  244 |         renderOption, maxAngularSize, color, opacity, scaleExponent, scaleFactor, up,
      |                                                       ^~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:244:70: error: 'scaleFactor' has not been declared
  244 |         renderOption, maxAngularSize, color, opacity, scaleExponent, scaleFactor, up,
      |                                                                      ^~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:244:83: error: 'up' has not been declared
  244 |         renderOption, maxAngularSize, color, opacity, scaleExponent, scaleFactor, up,
      |                                                                                   ^~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:245:9: error: 'right' has not been declared
  245 |         right, fadeInValue, hasSpriteTexture, spriteTexture, useTextureAlpha, useColorMap,
      |         ^~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:245:16: error: 'fadeInValue' has not been declared
  245 |         right, fadeInValue, hasSpriteTexture, spriteTexture, useTextureAlpha, useColorMap,
      |                ^~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:245:29: error: 'hasSpriteTexture' has not been declared
  245 |         right, fadeInValue, hasSpriteTexture, spriteTexture, useTextureAlpha, useColorMap,
      |                             ^~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:245:47: error: 'spriteTexture' has not been declared
  245 |         right, fadeInValue, hasSpriteTexture, spriteTexture, useTextureAlpha, useColorMap,
      |                                               ^~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:245:62: error: 'useTextureAlpha' has not been declared
  245 |         right, fadeInValue, hasSpriteTexture, spriteTexture, useTextureAlpha, useColorMap,
      |                                                              ^~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:245:79: error: 'useColorMap' has not been declared
  245 |         right, fadeInValue, hasSpriteTexture, spriteTexture, useTextureAlpha, useColorMap,
      |                                                                               ^~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:246:9: error: 'colorMapTexture' has not been declared
  246 |         colorMapTexture, cmapRangeMin, cmapRangeMax, nanColor, useNanColor,
      |         ^~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:246:26: error: 'cmapRangeMin' has not been declared
  246 |         colorMapTexture, cmapRangeMin, cmapRangeMax, nanColor, useNanColor,
      |                          ^~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:246:40: error: 'cmapRangeMax' has not been declared
  246 |         colorMapTexture, cmapRangeMin, cmapRangeMax, nanColor, useNanColor,
      |                                        ^~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:246:54: error: 'nanColor' has not been declared
  246 |         colorMapTexture, cmapRangeMin, cmapRangeMax, nanColor, useNanColor,
      |                                                      ^~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:246:64: error: 'useNanColor' has not been declared
  246 |         colorMapTexture, cmapRangeMin, cmapRangeMax, nanColor, useNanColor,
      |                                                                ^~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:247:9: error: 'hideOutsideRange' has not been declared
  247 |         hideOutsideRange, enableMaxSizeControl, aboveRangeColor, useAboveRangeColor,
      |         ^~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:247:27: error: 'enableMaxSizeControl' has not been declared
  247 |         hideOutsideRange, enableMaxSizeControl, aboveRangeColor, useAboveRangeColor,
      |                           ^~~~~~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:247:49: error: 'aboveRangeColor' has not been declared
  247 |         hideOutsideRange, enableMaxSizeControl, aboveRangeColor, useAboveRangeColor,
      |                                                 ^~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:247:66: error: 'useAboveRangeColor' has not been declared
  247 |         hideOutsideRange, enableMaxSizeControl, aboveRangeColor, useAboveRangeColor,
      |                                                                  ^~~~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:248:9: error: 'belowRangeColor' has not been declared
  248 |         belowRangeColor, useBelowRangeColor, hasDvarScaling, dvarScaleFactor, enableOutline,
      |         ^~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:248:26: error: 'useBelowRangeColor' has not been declared
  248 |         belowRangeColor, useBelowRangeColor, hasDvarScaling, dvarScaleFactor, enableOutline,
      |                          ^~~~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:248:46: error: 'hasDvarScaling' has not been declared
  248 |         belowRangeColor, useBelowRangeColor, hasDvarScaling, dvarScaleFactor, enableOutline,
      |                                              ^~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:248:62: error: 'dvarScaleFactor' has not been declared
  248 |         belowRangeColor, useBelowRangeColor, hasDvarScaling, dvarScaleFactor, enableOutline,
      |                                                              ^~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:248:79: error: 'enableOutline' has not been declared
  248 |         belowRangeColor, useBelowRangeColor, hasDvarScaling, dvarScaleFactor, enableOutline,
      |                                                                               ^~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:249:9: error: 'outlineColor' has not been declared
  249 |         outlineColor, outlineWeight, outlineStyle, useCmapOutline, aspectRatioScale,
      |         ^~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:249:23: error: 'outlineWeight' has not been declared
  249 |         outlineColor, outlineWeight, outlineStyle, useCmapOutline, aspectRatioScale,
      |                       ^~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:249:38: error: 'outlineStyle' has not been declared
  249 |         outlineColor, outlineWeight, outlineStyle, useCmapOutline, aspectRatioScale,
      |                                      ^~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:249:52: error: 'useCmapOutline' has not been declared
  249 |         outlineColor, outlineWeight, outlineStyle, useCmapOutline, aspectRatioScale,
      |                                                    ^~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:249:68: error: 'aspectRatioScale' has not been declared
  249 |         outlineColor, outlineWeight, outlineStyle, useCmapOutline, aspectRatioScale,
      |                                                                    ^~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:250:9: error: 'useOrientationData' is not a type
  250 |         useOrientationData
      |         ^~~~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:250:9: error: ISO C++ forbids declaration of 'useOrientationData' with no type [-fpermissive]
  250 |         useOrientationData
      |         ^~~~~~~~~~~~~~~~~~
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:241:5: error: expected ';' at end of member declaration
  241 |     UniformCache(
      |     ^~~~~~~~~~~~
In file included from /workspace/modules/base/rendering/pointcloud/renderableinterpolatedpoints.h:28,
                 from /workspace/modules/base/basemodule.cpp:48:
/workspace/modules/base/rendering/pointcloud/renderablepointcloud.h:251:7: error: '_uniformCacheFloat' does not name a type; did you mean 'UniformCacheBase'?
  251 |     ) _uniformCacheFloat;
      |       ^~~~~~~~~~~~~~~~~~
      |       UniformCacheBase
[320/1045] Building CXX object modules/atmosphere/CMakeFiles/openspace-module-atmosphere.dir/rendering/atmospheredeferredcaster.cpp.o
[321/1045] Building CXX object modules/atmosphere/CMakeFiles/openspace-module-atmosphere.dir/rendering/renderableatmosphere.cpp.o
[322/1045] Building CXX object modules/base/CMakeFiles/openspace-module-base.dir/dashboard/dashboarditemangle.cpp.o
ninja: build stopped: subcommand failed.
Error: Process completed with exit code 1.
```

### Prompt 21
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-24T08:06:37Z`
- **Completion Time (UTC)**: `2026-10-24T08:09:40Z`
- **Response Duration**: **3m 3s**

**Prompt:**
```text
Another build error, logs below.

[338/1045] Building CXX object modules/base/CMakeFiles/openspace-module-base.dir/dashboard/dashboarditemvelocity.cpp.o
[339/1045] Building CXX object modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderableboxgrid.cpp.o
FAILED: modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderableboxgrid.cpp.o 
/usr/bin/c++ -DCURL_STATICLIB -DD_GNU_SOURCE -DGLBINDING_AUX_STATIC_DEFINE -DGLBINDING_STATIC_DEFINE -DHAS_STRING_VIEW=1 -DONLY_C_LOCALE=0 -DOPENSPACE_DEBUG -DOPENSPACE_LOGGING_ENABLE_TRACE -DOPENSPACE_MODULE_ATMOSPHERE_ENABLED -DOPENSPACE_MODULE_AUDIO_ENABLED -DOPENSPACE_MODULE_BASE_ENABLED -DOPENSPACE_MODULE_CEFWEBGUI_ENABLED -DOPENSPACE_MODULE_DEBUGGING_ENABLED -DOPENSPACE_MODULE_DIGITALUNIVERSE_ENABLED -DOPENSPACE_MODULE_EXOPLANETS_ENABLED -DOPENSPACE_MODULE_FIELDLINESSEQUENCE_ENABLED -DOPENSPACE_MODULE_FIELDLINES_ENABLED -DOPENSPACE_MODULE_FITSFILEREADER_ENABLED -DOPENSPACE_MODULE_GAIA_ENABLED -DOPENSPACE_MODULE_GALAXY_ENABLED -DOPENSPACE_MODULE_GLOBEBROWSING_ENABLED -DOPENSPACE_MODULE_IMGUI_ENABLED -DOPENSPACE_MODULE_ISWA_ENABLED -DOPENSPACE_MODULE_KAMELEONVOLUME_ENABLED -DOPENSPACE_MODULE_KAMELEON_ENABLED -DOPENSPACE_MODULE_MOLECULE_ENABLED -DOPENSPACE_MODULE_MULTIRESVOLUME_ENABLED -DOPENSPACE_MODULE_OPENSOUNDCONTROL_ENABLED -DOPENSPACE_MODULE_SKYBROWSER_ENABLED -DOPENSPACE_MODULE_SOLARBROWSING_ENABLED -DOPENSPACE_MODULE_SPACECRAFTINSTRUMENTS_ENABLED -DOPENSPACE_MODULE_SPACE_ENABLED -DOPENSPACE_MODULE_STATEMACHINE_ENABLED -DOPENSPACE_MODULE_SYNC_ENABLED -DOPENSPACE_MODULE_TELEMETRY_ENABLED -DOPENSPACE_MODULE_TOUCH_ENABLED -DOPENSPACE_MODULE_VIDEO_ENABLED -DOPENSPACE_MODULE_VOLUME_ENABLED -DOPENSPACE_MODULE_WEBBROWSER_ENABLED -DOPENSPACE_MODULE_WEBGUI_ENABLED -DSYSTEM_LINUX -D_GLIBCXX_USE_TBB_PAR_BACKEND=0 -D_PSTL_PAR_BACKEND_SERIAL -I/workspace -I/workspace/include -I/workspace/build/_generated/include -isystem /vcpkg/installed/x64-linux/include -isystem /workspace/ext/renderdoc -isystem /vcpkg/installed/x64-linux/include/kubazip -O3 -DNDEBUG -std=gnu++23 -ggdb -march=x86-64-v3 -Wall -Wextra -Wpedantic -Walloc-zero -Wcast-qual -Wdate-time -Wduplicated-branches -Wduplicated-cond -Wenum-conversion -Wformat=2 -Wformat-signedness -Wimplicit-fallthrough -Winvalid-utf8 -Wlogical-op -Wmain -Wno-changes-meaning -Wshadow -Wundef -Wunused -Wuninitialized -Wvla -Wzero-as-null-pointer-constant -Wno-attributes -Wno-missing-field-initializers -DSCN_REGEX_BACKEND=0 -Winvalid-pch -include /workspace/build/modules/base/CMakeFiles/openspace-module-base.dir/cmake_pch.hxx -MD -MT modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderableboxgrid.cpp.o -MF modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderableboxgrid.cpp.o.d -o modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderableboxgrid.cpp.o -c /workspace/modules/base/rendering/grids/renderableboxgrid.cpp
/workspace/modules/base/rendering/grids/renderableboxgrid.cpp: In member function 'virtual void openspace::RenderableBoxGrid::initializeGL()':
/workspace/modules/base/rendering/grids/renderableboxgrid.cpp:124:21: error: 'const struct openspace::EnvCheckResult' has no member named 'isSet'
  124 |     if (noDoubleEnv.isSet) {
      |                     ^~~~~
In file included from /workspace/include/openspace/misc/objectmanager.inl:27,
                 from /workspace/include/openspace/misc/objectmanager.h:150,
                 from /workspace/include/openspace/opengl/programobjectmanager.h:28,
                 from /workspace/modules/base/basemodule.h:30,
                 from /workspace/modules/base/rendering/grids/renderableboxgrid.cpp:27:
/workspace/include/openspace/logging/logmanager.h:185:31: error: '_loggerCat' was not declared in this scope
  185 | #define LINFO(__msg__) LINFOC(_loggerCat, __msg__)
      |                               ^~~~~~~~~~
/workspace/modules/base/rendering/grids/renderableboxgrid.cpp:125:9: note: in expansion of macro 'LINFO'
  125 |         LINFO(std::format(
      |         ^~~~~
[340/1045] Building CXX object modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderablegrid.cpp.o
FAILED: modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderablegrid.cpp.o 
/usr/bin/c++ -DCURL_STATICLIB -DD_GNU_SOURCE -DGLBINDING_AUX_STATIC_DEFINE -DGLBINDING_STATIC_DEFINE -DHAS_STRING_VIEW=1 -DONLY_C_LOCALE=0 -DOPENSPACE_DEBUG -DOPENSPACE_LOGGING_ENABLE_TRACE -DOPENSPACE_MODULE_ATMOSPHERE_ENABLED -DOPENSPACE_MODULE_AUDIO_ENABLED -DOPENSPACE_MODULE_BASE_ENABLED -DOPENSPACE_MODULE_CEFWEBGUI_ENABLED -DOPENSPACE_MODULE_DEBUGGING_ENABLED -DOPENSPACE_MODULE_DIGITALUNIVERSE_ENABLED -DOPENSPACE_MODULE_EXOPLANETS_ENABLED -DOPENSPACE_MODULE_FIELDLINESSEQUENCE_ENABLED -DOPENSPACE_MODULE_FIELDLINES_ENABLED -DOPENSPACE_MODULE_FITSFILEREADER_ENABLED -DOPENSPACE_MODULE_GAIA_ENABLED -DOPENSPACE_MODULE_GALAXY_ENABLED -DOPENSPACE_MODULE_GLOBEBROWSING_ENABLED -DOPENSPACE_MODULE_IMGUI_ENABLED -DOPENSPACE_MODULE_ISWA_ENABLED -DOPENSPACE_MODULE_KAMELEONVOLUME_ENABLED -DOPENSPACE_MODULE_KAMELEON_ENABLED -DOPENSPACE_MODULE_MOLECULE_ENABLED -DOPENSPACE_MODULE_MULTIRESVOLUME_ENABLED -DOPENSPACE_MODULE_OPENSOUNDCONTROL_ENABLED -DOPENSPACE_MODULE_SKYBROWSER_ENABLED -DOPENSPACE_MODULE_SOLARBROWSING_ENABLED -DOPENSPACE_MODULE_SPACECRAFTINSTRUMENTS_ENABLED -DOPENSPACE_MODULE_SPACE_ENABLED -DOPENSPACE_MODULE_STATEMACHINE_ENABLED -DOPENSPACE_MODULE_SYNC_ENABLED -DOPENSPACE_MODULE_TELEMETRY_ENABLED -DOPENSPACE_MODULE_TOUCH_ENABLED -DOPENSPACE_MODULE_VIDEO_ENABLED -DOPENSPACE_MODULE_VOLUME_ENABLED -DOPENSPACE_MODULE_WEBBROWSER_ENABLED -DOPENSPACE_MODULE_WEBGUI_ENABLED -DSYSTEM_LINUX -D_GLIBCXX_USE_TBB_PAR_BACKEND=0 -D_PSTL_PAR_BACKEND_SERIAL -I/workspace -I/workspace/include -I/workspace/build/_generated/include -isystem /vcpkg/installed/x64-linux/include -isystem /workspace/ext/renderdoc -isystem /vcpkg/installed/x64-linux/include/kubazip -O3 -DNDEBUG -std=gnu++23 -ggdb -march=x86-64-v3 -Wall -Wextra -Wpedantic -Walloc-zero -Wcast-qual -Wdate-time -Wduplicated-branches -Wduplicated-cond -Wenum-conversion -Wformat=2 -Wformat-signedness -Wimplicit-fallthrough -Winvalid-utf8 -Wlogical-op -Wmain -Wno-changes-meaning -Wshadow -Wundef -Wunused -Wuninitialized -Wvla -Wzero-as-null-pointer-constant -Wno-attributes -Wno-missing-field-initializers -DSCN_REGEX_BACKEND=0 -Winvalid-pch -include /workspace/build/modules/base/CMakeFiles/openspace-module-base.dir/cmake_pch.hxx -MD -MT modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderablegrid.cpp.o -MF modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderablegrid.cpp.o.d -o modules/base/CMakeFiles/openspace-module-base.dir/rendering/grids/renderablegrid.cpp.o -c /workspace/modules/base/rendering/grids/renderablegrid.cpp
/workspace/modules/base/rendering/grids/renderablegrid.cpp: In member function 'virtual void openspace::RenderableGrid::initializeGL()':
/workspace/modules/base/rendering/grids/renderablegrid.cpp:232:21: error: 'const struct openspace::EnvCheckResult' has no member named 'isSet'
  232 |     if (noDoubleEnv.isSet) {
      |                     ^~~~~
In file included from /workspace/include/openspace/misc/objectmanager.inl:27,
                 from /workspace/include/openspace/misc/objectmanager.h:150,
                 from /workspace/include/openspace/opengl/programobjectmanager.h:28,
                 from /workspace/modules/base/basemodule.h:30,
                 from /workspace/modules/base/rendering/grids/renderablegrid.cpp:27:
/workspace/include/openspace/logging/logmanager.h:185:31: error: '_loggerCat' was not declared in this scope
  185 | #define LINFO(__msg__) LINFOC(_loggerCat, __msg__)
      |                               ^~~~~~~~~~
/workspace/modules/base/rendering/grids/renderablegrid.cpp:233:9: note: in expansion of macro 'LINFO'
  233 |         LINFO(std::format(
      |         ^~~~~
[341/1045] Building CXX object modules/base/CMakeFiles/openspace-module-base.dir/dashboard/dashboarditemtimevaryingtext.cpp.o
[342/1045] Building CXX object modules/base/CMakeFiles/openspace-module-base.dir/lightsource/scenegraphlightsource.cpp.o
ninja: build stopped: subcommand failed.
Error: Process completed with exit code 1.
```

### Prompt 22
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-24T08:52:13Z`
- **Completion Time (UTC)**: `2026-10-24T08:54:02Z`
- **Response Duration**: **1m 49s**

**Prompt:**
```text
Further build error,

[446/1045] Building CXX object modules/galaxy/CMakeFiles/openspace-module-galaxy.dir/cmake_pch.hxx.gch
[447/1045] Building CXX object modules/imgui/CMakeFiles/openspace-module-imgui.dir/cmake_pch.hxx.gch
[448/1045] Building CXX object modules/galaxy/CMakeFiles/openspace-module-galaxy.dir/rendering/galaxyraycaster.cpp.o
FAILED: modules/galaxy/CMakeFiles/openspace-module-galaxy.dir/rendering/galaxyraycaster.cpp.o 
/usr/bin/c++ -DCURL_STATICLIB -DD_GNU_SOURCE -DGLBINDING_AUX_STATIC_DEFINE -DGLBINDING_STATIC_DEFINE -DHAS_STRING_VIEW=1 -DONLY_C_LOCALE=0 -DOPENSPACE_DEBUG -DOPENSPACE_LOGGING_ENABLE_TRACE -DOPENSPACE_MODULE_ATMOSPHERE_ENABLED -DOPENSPACE_MODULE_AUDIO_ENABLED -DOPENSPACE_MODULE_BASE_ENABLED -DOPENSPACE_MODULE_CEFWEBGUI_ENABLED -DOPENSPACE_MODULE_DEBUGGING_ENABLED -DOPENSPACE_MODULE_DIGITALUNIVERSE_ENABLED -DOPENSPACE_MODULE_EXOPLANETS_ENABLED -DOPENSPACE_MODULE_FIELDLINESSEQUENCE_ENABLED -DOPENSPACE_MODULE_FIELDLINES_ENABLED -DOPENSPACE_MODULE_FITSFILEREADER_ENABLED -DOPENSPACE_MODULE_GAIA_ENABLED -DOPENSPACE_MODULE_GALAXY_ENABLED -DOPENSPACE_MODULE_GLOBEBROWSING_ENABLED -DOPENSPACE_MODULE_IMGUI_ENABLED -DOPENSPACE_MODULE_ISWA_ENABLED -DOPENSPACE_MODULE_KAMELEONVOLUME_ENABLED -DOPENSPACE_MODULE_KAMELEON_ENABLED -DOPENSPACE_MODULE_MOLECULE_ENABLED -DOPENSPACE_MODULE_MULTIRESVOLUME_ENABLED -DOPENSPACE_MODULE_OPENSOUNDCONTROL_ENABLED -DOPENSPACE_MODULE_SKYBROWSER_ENABLED -DOPENSPACE_MODULE_SOLARBROWSING_ENABLED -DOPENSPACE_MODULE_SPACECRAFTINSTRUMENTS_ENABLED -DOPENSPACE_MODULE_SPACE_ENABLED -DOPENSPACE_MODULE_STATEMACHINE_ENABLED -DOPENSPACE_MODULE_SYNC_ENABLED -DOPENSPACE_MODULE_TELEMETRY_ENABLED -DOPENSPACE_MODULE_TOUCH_ENABLED -DOPENSPACE_MODULE_VIDEO_ENABLED -DOPENSPACE_MODULE_VOLUME_ENABLED -DOPENSPACE_MODULE_WEBBROWSER_ENABLED -DOPENSPACE_MODULE_WEBGUI_ENABLED -DSYSTEM_LINUX -D_GLIBCXX_USE_TBB_PAR_BACKEND=0 -D_PSTL_PAR_BACKEND_SERIAL -I/workspace -I/workspace/include -I/workspace/build/_generated/include -isystem /vcpkg/installed/x64-linux/include -isystem /workspace/ext/renderdoc -isystem /vcpkg/installed/x64-linux/include/kubazip -O3 -DNDEBUG -std=gnu++23 -ggdb -march=x86-64-v3 -Wall -Wextra -Wpedantic -Walloc-zero -Wcast-qual -Wdate-time -Wduplicated-branches -Wduplicated-cond -Wenum-conversion -Wformat=2 -Wformat-signedness -Wimplicit-fallthrough -Winvalid-utf8 -Wlogical-op -Wmain -Wno-changes-meaning -Wshadow -Wundef -Wunused -Wuninitialized -Wvla -Wzero-as-null-pointer-constant -Wno-attributes -Wno-missing-field-initializers -DSCN_REGEX_BACKEND=0 -Winvalid-pch -include /workspace/build/modules/galaxy/CMakeFiles/openspace-module-galaxy.dir/cmake_pch.hxx -MD -MT modules/galaxy/CMakeFiles/openspace-module-galaxy.dir/rendering/galaxyraycaster.cpp.o -MF modules/galaxy/CMakeFiles/openspace-module-galaxy.dir/rendering/galaxyraycaster.cpp.o.d -o modules/galaxy/CMakeFiles/openspace-module-galaxy.dir/rendering/galaxyraycaster.cpp.o -c /workspace/modules/galaxy/rendering/galaxyraycaster.cpp
/workspace/modules/galaxy/rendering/galaxyraycaster.cpp: In member function 'void openspace::GalaxyRaycaster::initialize()':
/workspace/modules/galaxy/rendering/galaxyraycaster.cpp:67:9: error: 'LINFO' was not declared in this scope
   67 |         LINFO(std::format(
      |         ^~~~~
[449/1045] Building CXX object modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/cmake_pch.hxx.gch
[450/1045] Building CXX object modules/galaxy/CMakeFiles/openspace-module-galaxy.dir/galaxymodule.cpp.o
[451/1045] Building CXX object modules/iswa/CMakeFiles/openspace-module-iswa.dir/cmake_pch.hxx.gch
ninja: build stopped: subcommand failed.
Error: Process completed with exit code 1.
```

### Prompt 23
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-25T03:14:04Z`
- **Completion Time (UTC)**: `2026-10-25T03:16:57Z`
- **Response Duration**: **2m 53s**

**Prompt:**
```text
Next build error - 

[460/1045] Building CXX object modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/memoryawaretilecache.cpp.o
[461/1045] Building CXX object modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/renderableglobe.cpp.o
FAILED: modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/renderableglobe.cpp.o 
/usr/bin/c++ -DCURL_STATICLIB -DD_GNU_SOURCE -DGLBINDING_AUX_STATIC_DEFINE -DGLBINDING_STATIC_DEFINE -DH5_BUILT_AS_STATIC_LIB -DHAS_STRING_VIEW=1 -DHAVE_FENV -DNDEBUG -DONLY_C_LOCALE=0 -DOPENSPACE_DEBUG -DOPENSPACE_LOGGING_ENABLE_TRACE -DOPENSPACE_MODULE_ATMOSPHERE_ENABLED -DOPENSPACE_MODULE_AUDIO_ENABLED -DOPENSPACE_MODULE_BASE_ENABLED -DOPENSPACE_MODULE_CEFWEBGUI_ENABLED -DOPENSPACE_MODULE_DEBUGGING_ENABLED -DOPENSPACE_MODULE_DIGITALUNIVERSE_ENABLED -DOPENSPACE_MODULE_EXOPLANETS_ENABLED -DOPENSPACE_MODULE_FIELDLINESSEQUENCE_ENABLED -DOPENSPACE_MODULE_FIELDLINES_ENABLED -DOPENSPACE_MODULE_FITSFILEREADER_ENABLED -DOPENSPACE_MODULE_GAIA_ENABLED -DOPENSPACE_MODULE_GALAXY_ENABLED -DOPENSPACE_MODULE_GLOBEBROWSING_ENABLED -DOPENSPACE_MODULE_IMGUI_ENABLED -DOPENSPACE_MODULE_ISWA_ENABLED -DOPENSPACE_MODULE_KAMELEONVOLUME_ENABLED -DOPENSPACE_MODULE_KAMELEON_ENABLED -DOPENSPACE_MODULE_MOLECULE_ENABLED -DOPENSPACE_MODULE_MULTIRESVOLUME_ENABLED -DOPENSPACE_MODULE_OPENSOUNDCONTROL_ENABLED -DOPENSPACE_MODULE_SKYBROWSER_ENABLED -DOPENSPACE_MODULE_SOLARBROWSING_ENABLED -DOPENSPACE_MODULE_SPACECRAFTINSTRUMENTS_ENABLED -DOPENSPACE_MODULE_SPACE_ENABLED -DOPENSPACE_MODULE_STATEMACHINE_ENABLED -DOPENSPACE_MODULE_SYNC_ENABLED -DOPENSPACE_MODULE_TELEMETRY_ENABLED -DOPENSPACE_MODULE_TOUCH_ENABLED -DOPENSPACE_MODULE_VIDEO_ENABLED -DOPENSPACE_MODULE_VOLUME_ENABLED -DOPENSPACE_MODULE_WEBBROWSER_ENABLED -DOPENSPACE_MODULE_WEBGUI_ENABLED -DSYSTEM_LINUX -DUSE_UNSTABLE_GEOS_CPP_API -D_GLIBCXX_USE_TBB_PAR_BACKEND=0 -D_PSTL_PAR_BACKEND_SERIAL -I/workspace -I/workspace/include -I/workspace/build/_generated/include -isystem /vcpkg/installed/x64-linux/include -isystem /workspace/ext/renderdoc -isystem /vcpkg/installed/x64-linux/include/kubazip -isystem /vcpkg/installed/x64-linux/include/geos -O3 -DNDEBUG -std=gnu++23 -ggdb -march=x86-64-v3 -Wall -Wextra -Wpedantic -Walloc-zero -Wcast-qual -Wdate-time -Wduplicated-branches -Wduplicated-cond -Wenum-conversion -Wformat=2 -Wformat-signedness -Wimplicit-fallthrough -Winvalid-utf8 -Wlogical-op -Wmain -Wno-changes-meaning -Wshadow -Wundef -Wunused -Wuninitialized -Wvla -Wzero-as-null-pointer-constant -Wno-attributes -Wno-missing-field-initializers -DSCN_REGEX_BACKEND=0 -ffp-contract=off -Winvalid-pch -include /workspace/build/modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/cmake_pch.hxx -MD -MT modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/renderableglobe.cpp.o -MF modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/renderableglobe.cpp.o.d -o modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/renderableglobe.cpp.o -c /workspace/modules/globebrowsing/src/renderableglobe.cpp
/workspace/modules/globebrowsing/src/renderableglobe.cpp: In member function 'void openspace::RenderableGlobe::renderChunkGlobally(const openspace::Chunk&, const openspace::RenderData&, std::vector<DepthMapData>&, bool)':
/workspace/modules/globebrowsing/src/renderableglobe.cpp:1572:23: error: too many arguments to function 'std::pair<glm::mat<4, 4, float, glm::packed_highp>, glm::mat<4, 4, float, glm::packed_highp> > openspace::splitDmat4(const glm::dmat4&)'
 1572 |             splitDmat4(glm::inverse(data.camera.combinedViewMatrix()), inv_hi, inv_lo);
      |             ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
In file included from /workspace/modules/globebrowsing/src/ringscomponent.h:43,
                 from /workspace/modules/globebrowsing/src/renderableglobe.h:36,
                 from /workspace/modules/globebrowsing/src/renderableglobe.cpp:25:
/workspace/include/openspace/util/nogpudouble.h:80:40: note: declared here
   80 | inline std::pair<glm::mat4, glm::mat4> splitDmat4(const glm::dmat4& m) {
      |                                        ^~~~~~~~~~
/workspace/modules/globebrowsing/src/renderableglobe.cpp:1579:27: error: too many arguments to function 'std::pair<glm::mat<4, 4, float, glm::packed_highp>, glm::mat<4, 4, float, glm::packed_highp> > openspace::splitDmat4(const glm::dmat4&)'
 1579 |                 splitDmat4(lightViewProjections[i], lv_hi[i], lv_lo[i]);
      |                 ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/workspace/include/openspace/util/nogpudouble.h:80:40: note: declared here
   80 | inline std::pair<glm::mat4, glm::mat4> splitDmat4(const glm::dmat4& m) {
      |                                        ^~~~~~~~~~
/workspace/modules/globebrowsing/src/renderableglobe.cpp: In member function 'void openspace::RenderableGlobe::renderChunkLocally(const openspace::Chunk&, const openspace::RenderData&, std::vector<DepthMapData>&, bool)':
/workspace/modules/globebrowsing/src/renderableglobe.cpp:1832:23: error: too many arguments to function 'std::pair<glm::mat<4, 4, float, glm::packed_highp>, glm::mat<4, 4, float, glm::packed_highp> > openspace::splitDmat4(const glm::dmat4&)'
 1832 |             splitDmat4(glm::inverse(data.camera.combinedViewMatrix()), inv_hi, inv_lo);
      |             ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/workspace/include/openspace/util/nogpudouble.h:80:40: note: declared here
   80 | inline std::pair<glm::mat4, glm::mat4> splitDmat4(const glm::dmat4& m) {
      |                                        ^~~~~~~~~~
/workspace/modules/globebrowsing/src/renderableglobe.cpp:1839:27: error: too many arguments to function 'std::pair<glm::mat<4, 4, float, glm::packed_highp>, glm::mat<4, 4, float, glm::packed_highp> > openspace::splitDmat4(const glm::dmat4&)'
 1839 |                 splitDmat4(lightViewProjections[i], lv_hi[i], lv_lo[i]);
      |                 ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/workspace/include/openspace/util/nogpudouble.h:80:40: note: declared here
   80 | inline std::pair<glm::mat4, glm::mat4> splitDmat4(const glm::dmat4& m) {
      |                                        ^~~~~~~~~~
/workspace/modules/globebrowsing/src/renderableglobe.cpp: In member function 'void openspace::RenderableGlobe::setCommonUniforms(openspace::opengl::ProgramObject&, const openspace::Chunk&, const openspace::RenderData&)':
/workspace/modules/globebrowsing/src/renderableglobe.cpp:1958:19: error: too many arguments to function 'std::pair<glm::mat<4, 4, float, glm::packed_highp>, glm::mat<4, 4, float, glm::packed_highp> > openspace::splitDmat4(const glm::dmat4&)'
 1958 |         splitDmat4(_cachedModelTransform, m_hi, m_lo);
      |         ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/workspace/include/openspace/util/nogpudouble.h:80:40: note: declared here
   80 | inline std::pair<glm::mat4, glm::mat4> splitDmat4(const glm::dmat4& m) {
      |                                        ^~~~~~~~~~
/workspace/modules/globebrowsing/src/renderableglobe.cpp: In member function 'void openspace::RenderableGlobe::calculateEclipseShadows(openspace::opengl::ProgramObject&, const openspace::RenderData&, openspace::ShadowCompType)':
/workspace/modules/globebrowsing/src/renderableglobe.cpp:2546:27: error: too many arguments to function 'std::pair<glm::vec<3, float, glm::packed_highp>, glm::vec<3, float, glm::packed_highp> > openspace::splitDvec3(const glm::dvec3&)'
 2546 |                 splitDvec3(sd.casterPositionVec, pos_hi, pos_lo);
      |                 ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/workspace/include/openspace/util/nogpudouble.h:99:40: note: declared here
   99 | inline std::pair<glm::vec3, glm::vec3> splitDvec3(const glm::dvec3& v) {
      |                                        ^~~~~~~~~~
/workspace/modules/globebrowsing/src/renderableglobe.cpp:2563:23: error: too many arguments to function 'std::pair<glm::mat<4, 4, float, glm::packed_highp>, glm::mat<4, 4, float, glm::packed_highp> > openspace::splitDmat4(const glm::dmat4&)'
 2563 |             splitDmat4(glm::inverse(data.camera.combinedViewMatrix()), inv_hi, inv_lo);
      |             ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/workspace/include/openspace/util/nogpudouble.h:80:40: note: declared here
   80 | inline std::pair<glm::mat4, glm::mat4> splitDmat4(const glm::dmat4& m) {
      |                                        ^~~~~~~~~~
/workspace/modules/globebrowsing/src/renderableglobe.cpp:2574:23: error: too many arguments to function 'std::pair<glm::mat<4, 4, float, glm::packed_highp>, glm::mat<4, 4, float, glm::packed_highp> > openspace::splitDmat4(const glm::dmat4&)'
 2574 |             splitDmat4(_cachedModelTransform, m_hi, m_lo);
      |             ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/workspace/include/openspace/util/nogpudouble.h:80:40: note: declared here
   80 | inline std::pair<glm::mat4, glm::mat4> splitDmat4(const glm::dmat4& m) {
      |                                        ^~~~~~~~~~
[462/1045] Building CXX object modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/ringscomponent.cpp.o
FAILED: modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/ringscomponent.cpp.o 
/usr/bin/c++ -DCURL_STATICLIB -DD_GNU_SOURCE -DGLBINDING_AUX_STATIC_DEFINE -DGLBINDING_STATIC_DEFINE -DH5_BUILT_AS_STATIC_LIB -DHAS_STRING_VIEW=1 -DHAVE_FENV -DNDEBUG -DONLY_C_LOCALE=0 -DOPENSPACE_DEBUG -DOPENSPACE_LOGGING_ENABLE_TRACE -DOPENSPACE_MODULE_ATMOSPHERE_ENABLED -DOPENSPACE_MODULE_AUDIO_ENABLED -DOPENSPACE_MODULE_BASE_ENABLED -DOPENSPACE_MODULE_CEFWEBGUI_ENABLED -DOPENSPACE_MODULE_DEBUGGING_ENABLED -DOPENSPACE_MODULE_DIGITALUNIVERSE_ENABLED -DOPENSPACE_MODULE_EXOPLANETS_ENABLED -DOPENSPACE_MODULE_FIELDLINESSEQUENCE_ENABLED -DOPENSPACE_MODULE_FIELDLINES_ENABLED -DOPENSPACE_MODULE_FITSFILEREADER_ENABLED -DOPENSPACE_MODULE_GAIA_ENABLED -DOPENSPACE_MODULE_GALAXY_ENABLED -DOPENSPACE_MODULE_GLOBEBROWSING_ENABLED -DOPENSPACE_MODULE_IMGUI_ENABLED -DOPENSPACE_MODULE_ISWA_ENABLED -DOPENSPACE_MODULE_KAMELEONVOLUME_ENABLED -DOPENSPACE_MODULE_KAMELEON_ENABLED -DOPENSPACE_MODULE_MOLECULE_ENABLED -DOPENSPACE_MODULE_MULTIRESVOLUME_ENABLED -DOPENSPACE_MODULE_OPENSOUNDCONTROL_ENABLED -DOPENSPACE_MODULE_SKYBROWSER_ENABLED -DOPENSPACE_MODULE_SOLARBROWSING_ENABLED -DOPENSPACE_MODULE_SPACECRAFTINSTRUMENTS_ENABLED -DOPENSPACE_MODULE_SPACE_ENABLED -DOPENSPACE_MODULE_STATEMACHINE_ENABLED -DOPENSPACE_MODULE_SYNC_ENABLED -DOPENSPACE_MODULE_TELEMETRY_ENABLED -DOPENSPACE_MODULE_TOUCH_ENABLED -DOPENSPACE_MODULE_VIDEO_ENABLED -DOPENSPACE_MODULE_VOLUME_ENABLED -DOPENSPACE_MODULE_WEBBROWSER_ENABLED -DOPENSPACE_MODULE_WEBGUI_ENABLED -DSYSTEM_LINUX -DUSE_UNSTABLE_GEOS_CPP_API -D_GLIBCXX_USE_TBB_PAR_BACKEND=0 -D_PSTL_PAR_BACKEND_SERIAL -I/workspace -I/workspace/include -I/workspace/build/_generated/include -isystem /vcpkg/installed/x64-linux/include -isystem /workspace/ext/renderdoc -isystem /vcpkg/installed/x64-linux/include/kubazip -isystem /vcpkg/installed/x64-linux/include/geos -O3 -DNDEBUG -std=gnu++23 -ggdb -march=x86-64-v3 -Wall -Wextra -Wpedantic -Walloc-zero -Wcast-qual -Wdate-time -Wduplicated-branches -Wduplicated-cond -Wenum-conversion -Wformat=2 -Wformat-signedness -Wimplicit-fallthrough -Winvalid-utf8 -Wlogical-op -Wmain -Wno-changes-meaning -Wshadow -Wundef -Wunused -Wuninitialized -Wvla -Wzero-as-null-pointer-constant -Wno-attributes -Wno-missing-field-initializers -DSCN_REGEX_BACKEND=0 -ffp-contract=off -Winvalid-pch -include /workspace/build/modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/cmake_pch.hxx -MD -MT modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/ringscomponent.cpp.o -MF modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/ringscomponent.cpp.o.d -o modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/ringscomponent.cpp.o -c /workspace/modules/globebrowsing/src/ringscomponent.cpp
/workspace/modules/globebrowsing/src/ringscomponent.cpp: In member function 'void openspace::RingsComponent::draw(const openspace::RenderData&, const openspace::ShadowComponent::ShadowMapData&)':
/workspace/modules/globebrowsing/src/ringscomponent.cpp:498:23: error: too many arguments to function 'std::pair<glm::mat<4, 4, float, glm::packed_highp>, glm::mat<4, 4, float, glm::packed_highp> > openspace::splitDmat4(const glm::dmat4&)'
  498 |             splitDmat4(modelViewProjectionTransform, mvp_hi, mvp_lo);
      |             ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
In file included from /workspace/modules/globebrowsing/src/ringscomponent.h:43,
                 from /workspace/modules/globebrowsing/src/ringscomponent.cpp:25:
/workspace/include/openspace/util/nogpudouble.h:80:40: note: declared here
   80 | inline std::pair<glm::mat4, glm::mat4> splitDmat4(const glm::dmat4& m) {
      |                                        ^~~~~~~~~~
/workspace/modules/globebrowsing/src/ringscomponent.cpp:581:23: error: too many arguments to function 'std::pair<glm::mat<4, 4, float, glm::packed_highp>, glm::mat<4, 4, float, glm::packed_highp> > openspace::splitDmat4(const glm::dmat4&)'
  581 |             splitDmat4(modelViewProjectionTransform, mvp_hi, mvp_lo);
      |             ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/workspace/include/openspace/util/nogpudouble.h:80:40: note: declared here
   80 | inline std::pair<glm::mat4, glm::mat4> splitDmat4(const glm::dmat4& m) {
      |                                        ^~~~~~~~~~
[463/1045] Building CXX object modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/rawtiledatareader.cpp.o
[464/1045] Building CXX object modules/globebrowsing/CMakeFiles/openspace-module-globebrowsing.dir/src/shadowcomponent.cpp.o
ninja: build stopped: subcommand failed.
Error: Process completed with exit code 1.
```

### Prompt 24
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-25T03:55:30Z`
- **Completion Time (UTC)**: `2026-10-25T03:56:56Z`
- **Response Duration**: **1m 26s**

**Prompt:**
```text
Next build error,

[587/1045] Building CXX object modules/space/CMakeFiles/openspace-module-space.dir/spacemodule.cpp.o
[588/1045] Building CXX object modules/space/CMakeFiles/openspace-module-space.dir/kepler.cpp.o
[589/1045] Building CXX object modules/space/CMakeFiles/openspace-module-space.dir/horizonsfile.cpp.o
[590/1045] Building CXX object modules/space/CMakeFiles/openspace-module-space.dir/rendering/renderableconstellationlines.cpp.o
FAILED: modules/space/CMakeFiles/openspace-module-space.dir/rendering/renderableconstellationlines.cpp.o 
/usr/bin/c++ -DCURL_STATICLIB -DD_GNU_SOURCE -DGLBINDING_AUX_STATIC_DEFINE -DGLBINDING_STATIC_DEFINE -DHAS_STRING_VIEW=1 -DONLY_C_LOCALE=0 -DOPENSPACE_DEBUG -DOPENSPACE_LOGGING_ENABLE_TRACE -DOPENSPACE_MODULE_ATMOSPHERE_ENABLED -DOPENSPACE_MODULE_AUDIO_ENABLED -DOPENSPACE_MODULE_BASE_ENABLED -DOPENSPACE_MODULE_CEFWEBGUI_ENABLED -DOPENSPACE_MODULE_DEBUGGING_ENABLED -DOPENSPACE_MODULE_DIGITALUNIVERSE_ENABLED -DOPENSPACE_MODULE_EXOPLANETS_ENABLED -DOPENSPACE_MODULE_FIELDLINESSEQUENCE_ENABLED -DOPENSPACE_MODULE_FIELDLINES_ENABLED -DOPENSPACE_MODULE_FITSFILEREADER_ENABLED -DOPENSPACE_MODULE_GAIA_ENABLED -DOPENSPACE_MODULE_GALAXY_ENABLED -DOPENSPACE_MODULE_GLOBEBROWSING_ENABLED -DOPENSPACE_MODULE_IMGUI_ENABLED -DOPENSPACE_MODULE_ISWA_ENABLED -DOPENSPACE_MODULE_KAMELEONVOLUME_ENABLED -DOPENSPACE_MODULE_KAMELEON_ENABLED -DOPENSPACE_MODULE_MOLECULE_ENABLED -DOPENSPACE_MODULE_MULTIRESVOLUME_ENABLED -DOPENSPACE_MODULE_OPENSOUNDCONTROL_ENABLED -DOPENSPACE_MODULE_SKYBROWSER_ENABLED -DOPENSPACE_MODULE_SOLARBROWSING_ENABLED -DOPENSPACE_MODULE_SPACECRAFTINSTRUMENTS_ENABLED -DOPENSPACE_MODULE_SPACE_ENABLED -DOPENSPACE_MODULE_STATEMACHINE_ENABLED -DOPENSPACE_MODULE_SYNC_ENABLED -DOPENSPACE_MODULE_TELEMETRY_ENABLED -DOPENSPACE_MODULE_TOUCH_ENABLED -DOPENSPACE_MODULE_VIDEO_ENABLED -DOPENSPACE_MODULE_VOLUME_ENABLED -DOPENSPACE_MODULE_WEBBROWSER_ENABLED -DOPENSPACE_MODULE_WEBGUI_ENABLED -DSYSTEM_LINUX -D_GLIBCXX_USE_TBB_PAR_BACKEND=0 -D_PSTL_PAR_BACKEND_SERIAL -I/workspace -I/workspace/include -I/workspace/build/_generated/include -isystem /vcpkg/installed/x64-linux/include -isystem /workspace/ext/renderdoc -isystem /vcpkg/installed/x64-linux/include/kubazip -O3 -DNDEBUG -std=gnu++23 -ggdb -march=x86-64-v3 -Wall -Wextra -Wpedantic -Walloc-zero -Wcast-qual -Wdate-time -Wduplicated-branches -Wduplicated-cond -Wenum-conversion -Wformat=2 -Wformat-signedness -Wimplicit-fallthrough -Winvalid-utf8 -Wlogical-op -Wmain -Wno-changes-meaning -Wshadow -Wundef -Wunused -Wuninitialized -Wvla -Wzero-as-null-pointer-constant -Wno-attributes -Wno-missing-field-initializers -DSCN_REGEX_BACKEND=0 -Winvalid-pch -include /workspace/build/modules/space/CMakeFiles/openspace-module-space.dir/cmake_pch.hxx -MD -MT modules/space/CMakeFiles/openspace-module-space.dir/rendering/renderableconstellationlines.cpp.o -MF modules/space/CMakeFiles/openspace-module-space.dir/rendering/renderableconstellationlines.cpp.o.d -o modules/space/CMakeFiles/openspace-module-space.dir/rendering/renderableconstellationlines.cpp.o -c /workspace/modules/space/rendering/renderableconstellationlines.cpp
/workspace/modules/space/rendering/renderableconstellationlines.cpp: In member function 'virtual void openspace::RenderableConstellationLines::update(const openspace::UpdateData&)':
/workspace/modules/space/rendering/renderableconstellationlines.cpp:337:51: error: '_uniformCache' was not declared in this scope; did you mean 'UniformCache'?
  337 |         opengl::updateUniformLocations(*_program, _uniformCache);
      |                                                   ^~~~~~~~~~~~~
      |                                                   UniformCache
[591/1045] Building CXX object modules/space/CMakeFiles/openspace-module-space.dir/rendering/renderableconstellationsbase.cpp.o
[592/1045] Building CXX object modules/space/CMakeFiles/openspace-module-space.dir/rendering/renderableconstellationbounds.cpp.o
[593/1045] Building CXX object modules/space/CMakeFiles/openspace-module-space.dir/rendering/renderableeclipsecone.cpp.o
ninja: build stopped: subcommand failed.
Error: Process completed with exit code 1.
```

### Prompt 25
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-29T03:51:13Z`
- **Completion Time (UTC)**: `2026-10-29T04:00:25Z`
- **Response Duration**: **9m 12s**

**Prompt:**
```text
When this is built and tested on Windows, we get errors like this, 
Could not resolve file path for include file '${MODULE_BASE}/shaders/df64.glsl'
and so on for other paths like MODULE_GALAXY etc. Looking at the original glsl files, the include statements just are like
#include "df64.glsl"
so that needs to be fixed.

But after locally trying editing those include paths, then I get errors like
OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 71, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:20.372	OpenGL (Shader Compiler) [Error] {0}	Debug	Stacktrace
0: OpenSpace+0x877F7B
1: OpenSpace+0x848205
2: OpenSpace+0xAA2073
3: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E
4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B654
5: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB23
6: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F
7: OpenSpace+0xCB0708
8: OpenSpace+0xBD24CF
9: OpenSpace+0xBD04A5
10: OpenSpace+0x990567
11: OpenSpace!NCJunparse+0x1FA321E
12: OpenSpace!NCJunparse+0x1FA3682
13: OpenSpace+0xF274D0
14: OpenSpace!NCJunparse+0x1FA444A
15: OpenSpace!NCJunparse+0x1F381D7
16: OpenSpace+0xB8C82C
17: OpenSpace+0xB061C9
18: OpenSpace+0x99561D
19: OpenSpace+0x890126
20: OpenSpace+0x893A66
21: OpenSpace+0x7E7686
22: OpenSpace+0xD6106C
23: OpenSpace+0x7EBB46
24: OpenSpace!NCJunparse+0x1E6C42C
25: KERNEL32!BaseThreadInitThunk+0x17
26: ntdll!RtlUserThreadStart+0x2C
2026-10-28	20:56:20.378	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:20.378	SceneGraphNode	Debug	Initializing GL: MercuryLabel
2026-10-28	20:56:20.378	SceneGraphNode	Debug	Finished initializing GL: MercuryLabel
2026-10-28	20:56:20.378	SceneGraphNode	Debug	Initializing GL: VenusBarycenter
2026-10-28	20:56:20.378	SceneGraphNode	Debug	Finished initializing GL: VenusBarycenter
2026-10-28	20:56:20.378	SceneGraphNode	Debug	Initializing GL: Venus
2026-10-28	20:56:20.378	RenderableGlobe	Info	NO_GPU_DOUBLE environment variable detected. Using float shaders for RenderableGlobe.
2026-10-28	20:56:20.378	GlobeLabels	Info	Cached file 'D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\cache\venus.labels\4091483951\venus.labels' used for labels file 'D:\OpenSpace-0.19.2\OpenSpace-0.19.2\sync\http\venus_labels\1\venus.labels'
2026-10-28	20:56:20.482	SceneGraphNode	Debug	Finished initializing GL: Venus
2026-10-28	20:56:20.482	SceneGraphNode	Debug	Initializing GL: VenusTrail
2026-10-28	20:56:20.482	RenderableTrail	Info	NO_GPU_DOUBLE environment variable detected (set to '1'). Using float Trail shaders and uniforms.
2026-10-28	20:56:20.482	EphemerisProgramFloat	Debug	Creating object
2026-10-28	20:56:20.482	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 77, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:20.482	OpenGL (Shader Compiler) [Error] {0}	Debug	Stacktrace
0: OpenSpace+0x877F7B
1: OpenSpace+0x848205
2: OpenSpace+0xAA2073
3: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E
4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B654
5: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB23
6: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F
7: OpenSpace+0xCB0708
8: OpenSpace+0xBD24CF
9: OpenSpace+0xBD04A5
10: OpenSpace+0x990567
11: OpenSpace!NCJunparse+0x1FA321E
12: OpenSpace!NCJunparse+0x1FA3682
13: OpenSpace+0xF274D0
14: OpenSpace!NCJunparse+0x1FA444A
15: OpenSpace!NCJunparse+0x1F381D7
16: OpenSpace+0xB8C82C
17: OpenSpace+0xB061C9
18: OpenSpace+0x99561D
19: OpenSpace+0x890126
20: OpenSpace+0x893A66
21: OpenSpace+0x7E7686
22: OpenSpace+0xD6106C
23: OpenSpace+0x7EBB46
24: OpenSpace!NCJunparse+0x1E6C42C
25: KERNEL32!BaseThreadInitThunk+0x17
26: ntdll!RtlUserThreadStart+0x2C

and so on (230+ errors).
```

### Prompt 26
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-29T04:18:54Z`
- **Completion Time (UTC)**: `2026-10-29T04:21:52Z`
- **Response Duration**: **2m 58s**

**Prompt:**
```text
Then, how about deleting the extra unnecessary copies of df64.glsl, since  ${SHADERS} (OpenSpace/shaders/) is automatically registered in ShaderPreprocessor::includePaths() ?
```

### Prompt 27
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-29T04:23:37Z`
- **Completion Time (UTC)**: `2026-10-29T04:28:19Z`
- **Response Duration**: **4m 42s**

**Prompt:**
```text
Can you now check that all these errors have been resolved with the current canonical df64.glsl? 

2026-10-28	20:56:19.912	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 71, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:20.378	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:20.482	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 77, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:20.482	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:20.492	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 77, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:20.495	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:21.282	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 83, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:21.282	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:22.520	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 89, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:22.520	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:22.173	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 95, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:22.173	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:22.832	Cache	Error	Argument 'ModelProgram|float Vertex' contains an illegal character
2026-10-28	20:56:22.832	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 96, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:22.832	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:22.852	Cache	Error	Argument 'ModelProgram|float Vertex' contains an illegal character
2026-10-28	20:56:22.857	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 97, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:22.857	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:22.953	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 103, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:22.953	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:23.520	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 109, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:23.520	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:23.182	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 115, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:23.182	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:23.283	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 121, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:23.283	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:23.382	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 127, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:23.384	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:26.123	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 127, "AdvancedRingsProgramFloat Vertex": ERROR: 0:54: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:54: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:48: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:61: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:61: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:55: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:26.124	RingsComponent	Error	Error compiling shader object [AdvancedRingsProgramFloat Vertex]: ERROR: 0:54: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:54: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:48: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:61: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:61: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:55: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\advanced_rings_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\df64.glsl
2026-10-28	20:56:26.129	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 127, "RingsGeomOnlyProgramFloat Vertex": ERROR: 0:50: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:50: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:44: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:26.129	RingsComponent	Error	Error compiling shader object [RingsGeomOnlyProgramFloat Vertex]: ERROR: 0:50: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:50: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:44: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\rings_geom_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\df64.glsl
2026-10-28	20:56:26.252	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 133, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:26.253	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:26.349	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 139, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:26.349	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:26.459	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 145, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:26.460	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:26.539	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 151, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:26.540	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:26.639	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 157, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:26.639	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:26.737	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 163, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:26.737	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:26.833	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 169, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:26.833	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:26.934	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 175, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:26.934	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:27.622	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 181, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:27.622	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:27.722	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 187, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:27.722	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:27.798	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 193, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:27.798	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:27.874	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 199, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:27.874	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:27.952	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 205, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:27.952	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.320	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 211, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.320	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.112	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 217, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.112	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.202	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 223, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.202	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.305	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 229, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.305	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.382	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 235, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.382	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.485	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 241, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.485	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.485	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 241, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.485	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.582	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 247, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.582	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.662	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 253, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.662	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.740	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 259, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.741	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.812	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 265, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.812	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.894	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 271, "EphemerisProgramFloat Vertex": ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:28.894	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 0:109: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:109: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:103: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:28.932	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 272, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:28.932	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:28.942	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 272, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:28.942	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:28.948	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 272, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:28.952	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:28.952	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 272, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:28.952	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:28.952	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 272, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:28.962	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:29.239	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 275, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:29.240	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:30.984	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 275, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:30.992	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:30.998	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 275, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:30.998	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.270	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 278, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.270	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.320	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 278, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.320	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.320	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 278, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.320	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.750	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.750	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.770	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.770	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.850	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.850	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.900	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.910	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.920	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.960	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.960	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.960	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.102	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.102	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.107	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.107	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.107	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.107	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.112	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.112	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.112	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.112	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.112	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.122	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.122	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.126	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.130	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.131	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.135	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.136	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.140	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.140	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.143	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.143	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.143	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.143	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.152	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.152	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.152	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.152	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.162	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.162	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.162	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.162	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.175	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.175	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.175	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.175	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.182	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.182	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.192	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.192	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.196	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "GridProgramFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'

2026-10-28	20:56:31.196	ShaderObject	Error	Error compiling shader object [GridProgramFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:58: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:58: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:52: 'assign' : cannot convert from 'const highp float' to 'varying 4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\grid_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\df64.glsl
2026-10-28	20:56:31.202	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.202	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.207	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.207	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.212	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.212	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.212	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.212	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.222	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 281, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.222	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.232	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "RenderableDUMeshesFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.232	ShaderObject	Error	Error compiling shader object [RenderableDUMeshesFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\dumesh_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\df64.glsl
2026-10-28	20:56:31.238	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "RenderableDUMeshesFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.238	ShaderObject	Error	Error compiling shader object [RenderableDUMeshesFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\dumesh_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\df64.glsl
2026-10-28	20:56:31.242	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "RenderableDUMeshesFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.242	ShaderObject	Error	Error compiling shader object [RenderableDUMeshesFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\dumesh_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\df64.glsl
2026-10-28	20:56:31.242	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "RenderableDUMeshesFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.252	ShaderObject	Error	Error compiling shader object [RenderableDUMeshesFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\dumesh_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\df64.glsl
2026-10-28	20:56:31.254	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "RenderableDUMeshesFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.254	ShaderObject	Error	Error compiling shader object [RenderableDUMeshesFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\dumesh_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\df64.glsl
2026-10-28	20:56:31.262	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "RenderableDUMeshesFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.262	ShaderObject	Error	Error compiling shader object [RenderableDUMeshesFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\dumesh_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\df64.glsl
2026-10-28	20:56:31.262	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 280, "RenderableDUMeshesFloat Vertex": ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.262	ShaderObject	Error	Error compiling shader object [RenderableDUMeshesFloat Vertex]: ERROR: 0:48: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:48: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:42: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\dumesh_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\digitaluniverse\shaders\df64.glsl
2026-10-28	20:56:31.427	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 289, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.427	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.432	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 289, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.432	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.438	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 289, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.438	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.442	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 289, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'

2026-10-28	20:56:31.442	ShaderObject	Error	Error compiling shader object [RenderablePointCloudFloat Geometry]: ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:133: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:133: 'df64_vec3_sub' : function is not known
ERROR: 0:127: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:159: 'df64_vec3_sub' : no matching overloaded function found (using implicit conversion)
ERROR: 0:159: 'df64_vec3_sub' : function is not known
ERROR: 0:153: '=' : cannot convert from 'const highp float' to '3-component vector of highp float'
ERROR: 0:177: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:177: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:171: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:187: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:187: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:181: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'
ERROR: 0:195: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:195: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:189: '=' : cannot convert from 'const highp float' to '4-component vector of highp float'


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\pointcloud\pointcloud_gs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscalingmath.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-28	20:56:31.449	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 289, "RenderablePointCloudFloat Geometry": ERROR: 0:113: 'df64_mat4_mul_vec4' : no matching overloaded function found (using implicit conversion)
ERROR: 0:113: 'df64_mat4_mul_vec4' : function is not known
ERROR: 0:107: '=' : cannot convert from 'const highp floa
<truncated 52212 bytes>

NOTE: The output was truncated because it was too long. Use a more targeted query or a smaller range to get the information you need.
```

### Prompt 28
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-29T04:37:05Z`
- **Completion Time (UTC)**: `2026-10-29T04:37:26Z`
- **Response Duration**: **21s**

**Prompt:**
```text
Please list the paths to all the files deleted and all the files added or changed in the last 24 hours in this session, so that I can drag and drop them into github.
```

### Prompt 29
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-30T03:35:43Z`
- **Completion Time (UTC)**: `2026-10-30T03:38:45Z`
- **Response Duration**: **3m 2s**

**Prompt:**
```text
Now I get errors like this. Please check how the other shaders in OpenSpace/shaders avoid such duplication errors, and follow a similar strategy.

2026-10-29	17:16:14.566	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 53, "LocalChunkedLodPatchFloat Vertex": ERROR: 8:207: 'df64_vec3_sub' : function already has a body
ERROR: 8:223: 'df64_vec3_add' : function already has a body

2026-10-29	17:16:15.152	OpenGL (Shader Compiler) [Error] {0}	Debug	Stacktrace
0: OpenSpace+0x877F7B
1: OpenSpace+0x848205
2: OpenSpace+0xAA2073
3: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E
4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B654
5: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB23
6: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F
7: OpenSpace+0xCB0708
8: OpenSpace+0xBD24CF
9: OpenSpace+0xBD04A5
10: OpenSpace+0x990567
11: OpenSpace+0x16681A3
12: OpenSpace+0x1665E1A
13: OpenSpace+0xB8C82C
14: OpenSpace+0xB061C9
15: OpenSpace+0x99561D
16: OpenSpace+0x890126
17: OpenSpace+0x893A66
18: OpenSpace+0x7E7686
19: OpenSpace+0xD6106C
20: OpenSpace+0x7EBB46
21: OpenSpace!NCJunparse+0x1E6C42C
22: KERNEL32!BaseThreadInitThunk+0x17
23: ntdll!RtlUserThreadStart+0x2C
2026-10-29	17:16:15.162	ShaderObject	Error	Error compiling shader object [LocalChunkedLodPatchFloat Vertex]: ERROR: 8:207: 'df64_vec3_sub' : function already has a body
ERROR: 8:223: 'df64_vec3_add' : function already has a body


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\localrenderer_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\tile.glsl
4: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\texturetilemapping.glsl
5: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\blending.glsl
6: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\tileheight.glsl
7: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\tilevertexskirt.glsl
8: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-29	17:16:15.162	SceneGraphNode	Debug	Initializing GL: SunGlare
2026-10-29	17:16:15.162	Plane	Debug	Creating object
2026-10-29	17:16:15.162	FileSystem	Debug	Started watching 'D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders'
2026-10-29	17:16:15.212	4013050064	Debug	Creating object
2026-10-29	17:16:15.278	RenderablePlaneImageLocal	Debug	Loaded texture from 'D:\OpenSpace-0.19.2\OpenSpace-0.19.2\sync\http\sun_textures\4\halo.png'
2026-10-29	17:16:15.282	SceneGraphNode	Debug	Finished initializing GL: SunGlare
2026-10-29	17:16:15.282	SceneGraphNode	Debug	Initializing GL: SunLabel
2026-10-29	17:16:15.282	SceneGraphNode	Debug	Finished initializing GL: SunLabel
2026-10-29	17:16:15.282	SceneGraphNode	Debug	Initializing GL: SunHabitableZone
2026-10-29	17:16:15.289	FileSystem	Debug	Started watching 'D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\space\shaders'
2026-10-29	17:16:15.349	TextureComponent	Debug	Loaded texture from 'D:\OpenSpace-0.19.2\OpenSpace-0.19.2\sync\http\habitable_zone_textures\1\hot_to_cold_faded.png'
2026-10-29	17:16:15.349	FileSystem	Debug	Started watching 'D:\OpenSpace-0.19.2\OpenSpace-0.19.2\sync\http\habitable_zone_textures\1'
2026-10-29	17:16:15.349	SceneGraphNode	Debug	Finished initializing GL: SunHabitableZone
2026-10-29	17:16:15.349	SceneGraphNode	Debug	Initializing GL: MercuryBarycenter
2026-10-29	17:16:15.349	SceneGraphNode	Debug	Finished initializing GL: MercuryBarycenter
2026-10-29	17:16:15.349	SceneGraphNode	Debug	Initializing GL: Mercury
2026-10-29	17:16:15.349	RenderableGlobe	Info	NO_GPU_DOUBLE environment variable detected. Using float shaders for RenderableGlobe.
2026-10-29	17:16:15.349	GlobeLabels	Info	Cached file 'D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\cache\Mercury.labels\1407167935\Mercury.labels' used for labels file 'D:\OpenSpace-0.19.2\OpenSpace-0.19.2\sync\http\mercury_labels\1\Mercury.labels'
2026-10-29	17:16:15.382	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 59, "LocalChunkedLodPatchFloat Vertex": ERROR: 8:207: 'df64_vec3_sub' : function already has a body
ERROR: 8:223: 'df64_vec3_add' : function already has a body

2026-10-29	17:16:15.382	OpenGL (Shader Compiler) [Error] {0}	Debug	Stacktrace
0: OpenSpace+0x877F7B
1: OpenSpace+0x848205
2: OpenSpace+0xAA2073
3: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E
4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B654
5: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB23
6: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F
7: OpenSpace+0xCB0708
8: OpenSpace+0xBD24CF
9: OpenSpace+0xBD04A5
10: OpenSpace+0x990567
11: OpenSpace+0x16681A3
12: OpenSpace+0x1665E1A
13: OpenSpace+0xB8C82C
14: OpenSpace+0xB061C9
15: OpenSpace+0x99561D
16: OpenSpace+0x890126
17: OpenSpace+0x893A66
18: OpenSpace+0x7E7686
19: OpenSpace+0xD6106C
20: OpenSpace+0x7EBB46
21: OpenSpace!NCJunparse+0x1E6C42C
22: KERNEL32!BaseThreadInitThunk+0x17
23: ntdll!RtlUserThreadStart+0x2C
2026-10-29	17:16:15.382	ShaderObject	Error	Error compiling shader object [LocalChunkedLodPatchFloat Vertex]: ERROR: 8:207: 'df64_vec3_sub' : function already has a body
ERROR: 8:223: 'df64_vec3_add' : function already has a body


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\localrenderer_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\tile.glsl
4: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\texturetilemapping.glsl
5: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\blending.glsl
6: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\tileheight.glsl
7: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\tilevertexskirt.glsl
8: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-29	17:16:15.382	SceneGraphNode	Debug	Initializing GL: MercuryTrail
2026-10-29	17:16:15.386	RenderableTrail	Info	NO_GPU_DOUBLE environment variable detected (set to '1'). Using float Trail shaders and uniforms.
2026-10-29	17:16:15.386	EphemerisProgramFloat	Debug	Creating object
2026-10-29	17:16:15.394	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 59, "EphemerisProgramFloat Vertex": ERROR: 3:207: 'df64_vec3_sub' : function already has a body
ERROR: 3:223: 'df64_vec3_add' : function already has a body

2026-10-29	17:16:15.396	OpenGL (Shader Compiler) [Error] {0}	Debug	Stacktrace
0: OpenSpace+0x877F7B
1: OpenSpace+0x848205
2: OpenSpace+0xAA2073
3: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E
4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B654
5: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB23
6: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F
7: OpenSpace+0xCB0708
8: OpenSpace+0xBD24CF
9: OpenSpace+0xBD04A5
10: OpenSpace+0x990567
11: OpenSpace!NCJunparse+0x1FA33BE
12: OpenSpace!NCJunparse+0x1FA3822
13: OpenSpace+0xF274D0
14: OpenSpace!NCJunparse+0x1FA45EA
15: OpenSpace!NCJunparse+0x1F38377
16: OpenSpace+0xB8C82C
17: OpenSpace+0xB061C9
18: OpenSpace+0x99561D
19: OpenSpace+0x890126
20: OpenSpace+0x893A66
21: OpenSpace+0x7E7686
22: OpenSpace+0xD6106C
23: OpenSpace+0x7EBB46
24: OpenSpace!NCJunparse+0x1E6C42C
25: KERNEL32!BaseThreadInitThunk+0x17
26: ntdll!RtlUserThreadStart+0x2C
2026-10-29	17:16:15.397	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 3:207: 'df64_vec3_sub' : function already has a body
ERROR: 3:223: 'df64_vec3_add' : function already has a body


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-29	17:16:15.397	SceneGraphNode	Debug	Initializing GL: MercuryLabel
2026-10-29	17:16:15.397	SceneGraphNode	Debug	Finished initializing GL: MercuryLabel
2026-10-29	17:16:15.397	SceneGraphNode	Debug	Initializing GL: VenusBarycenter
2026-10-29	17:16:15.397	SceneGraphNode	Debug	Finished initializing GL: VenusBarycenter
2026-10-29	17:16:15.397	SceneGraphNode	Debug	Initializing GL: Venus
2026-10-29	17:16:15.397	RenderableGlobe	Info	NO_GPU_DOUBLE environment variable detected. Using float shaders for RenderableGlobe.
2026-10-29	17:16:15.397	GlobeLabels	Info	Cached file 'D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\cache\venus.labels\4091483951\venus.labels' used for labels file 'D:\OpenSpace-0.19.2\OpenSpace-0.19.2\sync\http\venus_labels\1\venus.labels'
2026-10-29	17:16:15.428	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 59, "LocalChunkedLodPatchFloat Vertex": ERROR: 8:207: 'df64_vec3_sub' : function already has a body
ERROR: 8:223: 'df64_vec3_add' : function already has a body

2026-10-29	17:16:15.428	OpenGL (Shader Compiler) [Error] {0}	Debug	Stacktrace
0: OpenSpace+0x877F7B
1: OpenSpace+0x848205
2: OpenSpace+0xAA2073
3: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E
4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B654
5: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB23
6: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F
7: OpenSpace+0xCB0708
8: OpenSpace+0xBD24CF
9: OpenSpace+0xBD04A5
10: OpenSpace+0x990567
11: OpenSpace+0x16681A3
12: OpenSpace+0x1665E1A
13: OpenSpace+0xB8C82C
14: OpenSpace+0xB061C9
15: OpenSpace+0x99561D
16: OpenSpace+0x890126
17: OpenSpace+0x893A66
18: OpenSpace+0x7E7686
19: OpenSpace+0xD6106C
20: OpenSpace+0x7EBB46
21: OpenSpace!NCJunparse+0x1E6C42C
22: KERNEL32!BaseThreadInitThunk+0x17
23: ntdll!RtlUserThreadStart+0x2C
2026-10-29	17:16:15.428	ShaderObject	Error	Error compiling shader object [LocalChunkedLodPatchFloat Vertex]: ERROR: 8:207: 'df64_vec3_sub' : function already has a body
ERROR: 8:223: 'df64_vec3_add' : function already has a body


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\localrenderer_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\tile.glsl
4: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\texturetilemapping.glsl
5: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\blending.glsl
6: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\tileheight.glsl
7: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\globebrowsing\shaders\tilevertexskirt.glsl
8: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl
2026-10-29	17:16:15.428	SceneGraphNode	Debug	Initializing GL: VenusTrail
2026-10-29	17:16:15.428	RenderableTrail	Info	NO_GPU_DOUBLE environment variable detected (set to '1'). Using float Trail shaders and uniforms.
2026-10-29	17:16:15.428	EphemerisProgramFloat	Debug	Creating object
2026-10-29	17:16:15.436	OpenGL (Shader Compiler) [Error] {0}	Error	SHADER_ID_COMPILE error has been generated. GLSL compile failed for shader 59, "EphemerisProgramFloat Vertex": ERROR: 3:207: 'df64_vec3_sub' : function already has a body
ERROR: 3:223: 'df64_vec3_add' : function already has a body

2026-10-29	17:16:15.436	OpenGL (Shader Compiler) [Error] {0}	Debug	Stacktrace
0: OpenSpace+0x877F7B
1: OpenSpace+0x848205
2: OpenSpace+0xAA2073
3: igxelpicd64!DumpRegistryKeyDefinitions+0x6B41E
4: igxelpicd64!DumpRegistryKeyDefinitions+0x6B654
5: igxelpicd64!DumpRegistryKeyDefinitions+0x6BB23
6: igxelpicd64!DumpRegistryKeyDefinitions+0x7BDE9F
7: OpenSpace+0xCB0708
8: OpenSpace+0xBD24CF
9: OpenSpace+0xBD04A5
10: OpenSpace+0x990567
11: OpenSpace!NCJunparse+0x1FA33BE
12: OpenSpace!NCJunparse+0x1FA3822
13: OpenSpace+0xF274D0
14: OpenSpace!NCJunparse+0x1FA45EA
15: OpenSpace!NCJunparse+0x1F38377
16: OpenSpace+0xB8C82C
17: OpenSpace+0xB061C9
18: OpenSpace+0x99561D
19: OpenSpace+0x890126
20: OpenSpace+0x893A66
21: OpenSpace+0x7E7686
22: OpenSpace+0xD6106C
23: OpenSpace+0x7EBB46
24: OpenSpace!NCJunparse+0x1E6C42C
25: KERNEL32!BaseThreadInitThunk+0x17
26: ntdll!RtlUserThreadStart+0x2C
2026-10-29	17:16:15.436	ShaderObject	Error	Error compiling shader object [EphemerisProgramFloat Vertex]: ERROR: 3:207: 'df64_vec3_sub' : function already has a body
ERROR: 3:223: 'df64_vec3_add' : function already has a body


0: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\modules\base\shaders\renderabletrail_vs_float.glsl
1: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling/powerscaling_vs.glsl
2: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\powerscaling\powerscalingmath.glsl
3: D:\Downloads\OpenSpace-minimal-test-vcpkg-fp64-emu\shaders\df64.glsl

and so on, 300+ similar errors
```

### Prompt 30
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-30T07:37:26Z`
- **Completion Time (UTC)**: `2026-10-30T07:39:06Z`
- **Response Duration**: **1m 40s**

**Prompt:**
```text
After fixing that, now the errors are:

2026-10-30	12:37:57.206	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 283, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.586	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.616	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 283, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.616	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.856	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 286, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.856	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.865	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 286, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.865	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.874	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 286, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.874	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.876	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 286, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:57.876	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.626	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 286, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.626	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.637	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 286, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.640	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.674	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 289, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.676	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.679	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 289, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.679	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.686	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 289, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.686	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.755	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.755	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.766	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.766	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.766	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.766	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.786	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.786	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.791	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.791	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.796	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.796	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.809	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.809	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.816	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.816	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.822	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.822	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.826	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.826	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.841	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.841	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.848	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.848	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.856	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.856	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.856	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 295, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:37:59.856	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.660	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.660	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.730	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.750	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.760	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.760	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.860	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.860	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.960	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.960	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.103	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.103	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.107	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.107	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.507	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.507	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.536	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.536	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.541	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.541	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.546	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.546	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.556	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.556	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.561	OpenGL (Shader Compiler) [Error] {1}	Error	SHADER_ID_LINK error has been generated. GLSL link failed for program 306, "RenderablePointCloudFloat": Varying "Data;_IN" has different block does not match across different shaders.
2026-10-30	12:38:00.561	ProgramObject	Error	Error linking program object [RenderablePointCloudFloat]: Varying "Data;_IN" has different block does not match across different shaders.
```

### Prompt 31
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-31T03:14:50Z`
- **Completion Time (UTC)**: `2026-10-31T03:21:40Z`
- **Response Duration**: **6m 50s**

**Prompt:**
```text
Now those errors are gone. OpenSpace does run. But the renderabletrails don't display if we use NO_GPU_DOUBLE=1.
```

### Prompt 32
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-10-31T03:29:32Z`
- **Completion Time (UTC)**: `2026-10-31T03:39:18Z`
- **Response Duration**: **9m 46s**

**Prompt:**
```text
Can you check all the "renderable" files for such inconsistencies between the original and ...float shaders?
```

### Prompt 33
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-11-01T08:31:28Z`
- **Completion Time (UTC)**: `2026-11-01T08:42:00Z`
- **Response Duration**: **10m 32s**

**Prompt:**
```text
I'm trying to test OpenSpace running with Dekker Veltkamp fp64 emulation in the shaders versus using doubles in shader uniforms (not supported in hardware by many GPUs). When I tested on Windows with Intel GPU and NO_GPU_DOUBLE=1, the Tully galaxies asset of OpenSpace was being rendered, but with some differences from the NO_GPU_DOUBLE=0 original version. Testing now on Linux, NVidia GPU, and NO_GPU_DOUBLE=1, The Tully galaxies are not being rendered at all.

On Linux, these warnings are generated
The log showed only these warnings, but possibly relevant - 

2026-11-01	07:55:27.123	ProgramObject('Deferred 0 raycast')	Warning	Fragment info
-------------
0(467) : warning C7050: "posObj_m.hi" might be used before being initialized
0(467) : warning C7050: "posObj_m.lo" might be used before being initialized
2026-11-01	07:55:27.123	AtmosphereDeferredcaster	Info	Loading Atmosphere deferred fragment shader: /home/sssvv/.local/share/OpenSpace/0.22.0-dev/modules/atmosphere/shaders/atmosphere_deferred_fs_float.glsl
2026-11-01	07:55:27.128	ProgramObject('Deferred 1 raycast')	Warning	Fragment info
-------------
0(467) : warning C7050: "posObj_m.hi" might be used before being initialized
0(467) : warning C7050: "posObj_m.lo" might be used before being initialized
2026-11-01	07:55:27.128	AtmosphereDeferredcaster	Info	Loading Atmosphere deferred fragment shader: /home/sssvv/.local/share/OpenSpace/0.22.0-dev/modules/atmosphere/shaders/atmosphere_deferred_fs_float.glsl
2026-11-01	07:55:27.133	ProgramObject('Deferred 2 raycast')	Warning	Fragment info
-------------
0(467) : warning C7050: "posObj_m.hi" might be used before being initialized
0(467) : warning C7050: "posObj_m.lo" might be used before being initialized
2026-11-01	07:55:27.134	AtmosphereDeferredcaster	Info	Loading Atmosphere deferred fragment shader: /home/sssvv/.local/share/OpenSpace/0.22.0-dev/modules/atmosphere/shaders/atmosphere_deferred_fs_float.glsl
2026-11-01	07:55:27.139	ProgramObject('Deferred 3 raycast')	Warning	Fragment info
-------------
0(467) : warning C7050: "posObj_m.hi" might be used before being initialized
0(467) : warning C7050: "posObj_m.lo" might be used before being initialized
2026-11-01	07:55:27.139	Logging	Warning	Number of Warnings: 4

Claude says,

Those warnings are useful, but they come from the atmosphere shader (atmosphere_deferred_fs_float.glsl), not RenderablePointCloud, so they’re unlikely to be why the galaxies are missing. They do point at a real bug that fits your Intel-vs-NVIDIA difference.

What the warning means

C7050 is NVIDIA’s compiler saying that posObj_m.hi and posObj_m.lo can be read on some code path before anything has been written to them. That typically happens when:

a struct is declared (dvec3_emu posObj_m;) and only assigned inside a branch, or
an out/inout struct parameter is only partially assigned by an emulation helper.

Uninitialized locals are undefined in GLSL. Intel’s driver often happens to give you zeros, while NVIDIA may give garbage or NaN. That fits “mostly works on Intel with small differences” and “breaks on NVIDIA”. A NaN in a position that feeds the final transform silently produces no visible output.

What to do

Fix the atmosphere one. The line number (467) refers to the assembled shader after #includes are expanded, not the file on disk. Find the declaration of posObj_m in atmosphere_deferred_fs_float.glsl and its includes, and initialize it explicitly, e.g. posObj_m.hi = vec3(0.0); posObj_m.lo = vec3(0.0); (or use a constructor). Also check that every branch assigns both hi and lo.
Hunt for the same pattern in the point cloud path. The point cloud shaders produced no warnings, which tells you two things: they compiled and linked (so a compile failure isn’t your problem), and the compiler didn’t catch an uninitialized struct there. NVIDIA’s warning only fires for patterns it can detect statically, so don’t treat silence as proof. Grep the emulation helpers and the renderablepointcloud / billboardpoint shaders for emulated-type locals that aren’t fully initialized, especially in out parameters.
Since compilation is fine, focus on runtime values. The most productive test is the one from before: in the point cloud vertex shader, bypass the emulated position math and write a hardcoded gl_Position and a constant fragment color. If points appear, the problem is NaN or garbage coming out of the hi/lo math (or its uniforms). If nothing appears, look at geometry emission or draw calls instead.
Check the uniforms. If the emulated path expects *_hi/*_lo uniforms and the C++ side sets them under a different name, the uniform location is -1 and the value silently stays zero. OpenSpace usually logs missing uniforms only at debug verbosity, so raise the log level if you haven’t.
```

### Prompt 34
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-11-02T07:38:54Z`
- **Completion Time (UTC)**: `2026-11-02T07:46:28Z`
- **Response Duration**: **7m 34s**

**Prompt:**
```text
The "Tully Galaxy Images" are rendering fine on Windows+Intel and Linux+NVidia. The "Tully Galaxies" are not rendering in NO_GPU_DOUBLE=1 mode on both Windows+Intel and Linux+NVidia.
```

### Prompt 35
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-11-02T08:11:52Z`
- **Completion Time (UTC)**: `2026-11-02T08:17:03Z`
- **Response Duration**: **5m 11s**

**Prompt:**
```text
This seems to have fixed the problem, thank you. Now I would like to run all the visual tests available. Please give me a python script similar to the one in the OpenSpace repository support/runner/main.py but customized for Linux - where the command 
openspace
will run OpenSpace since it is a wrapper available in the path.
Additionally, please add an option to the script to run all the tests which use the empty profile in "dry run" mode without taking screenshots, waiting for user with press any key or something like that,  without closing and opening OpenSpace everytime so that I can fill up the MRF cache.
```

### Prompt 36
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-11-02T08:52:15Z`
- **Completion Time (UTC)**: `2026-11-02T08:55:26Z`
- **Response Duration**: **3m 11s**

**Prompt:**
```text
In -a mode, when we run multiple tests, the copy command is copying all the pngs of all the tests done so far into the destination filename, overwriting the destination multiple times.
```

### Prompt 37
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-11-02T08:57:02Z`
- **Completion Time (UTC)**: `2026-11-02T08:57:02Z`
- **Response Duration**: **0s**

**Prompt:**
```text
Would not a simple replacement of the copy command with a move command in the earlier script solve this problem?
```

### Prompt 38
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-11-03T03:36:41Z`
- **Completion Time (UTC)**: `2026-11-03T03:47:40Z`
- **Response Duration**: **10m 59s**

**Prompt:**
```text
Now, the fp64 emulation works well. But the OpenSpace master branch has moved on. The current OpenSpace master branch is cloned into the project directory as OpenSpace-current-master 

Please generate a strategy by which the current master can be patched - possibly using git apply with the flag to ignore line number changes and whitespace changes - to produce the fp64 emulated version with the same behaviour as the working code - ie if the environment variable NO_GPU_DOUBLE=1, then the ...float.glsl shaders are used, and if the variable is not set or is set to 0, the regular OpenSpace shaders are used.

I have now created a directory called v0-22-1-patches in the working directory of this project. Please put the patches and the patching instructions into this directory. I will later take the patches from there, upload them to a github repo, and run a workflow on github to build OpenSpace using the patches.

Don't try to build on this machine, since this is a Mac and the build needs to be run on Windows or Linux. Just create the patches and the patching instructions.
```

### Prompt 39
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-11-04T04:49:07Z`
- **Completion Time (UTC)**: `2026-11-04T05:03:59Z`
- **Response Duration**: **14m 52s**

**Prompt:**
```text
Doing visual regression tests between the NO_GPU_DOUBLE=1 and NO_GPU_DOUBLE=0 renderings, I see that the asset "Milky Way Volume" is rendered in the NO_GPU_DOUBLE=0 in a more crisp way, while the NO_GPU_DOUBLE=1 version seems softer and out of focus.
```

### Prompt 40
- **Model Used**: Gemini 3.8 Flash (Medium)
- **Start Time (UTC)**: `2026-11-05T03:25:49Z`
- **Completion Time (UTC)**: `In progress`
- **Response Duration**: **Current turn (generating Prompts.md)**

**Prompt:**
```text
Can you make a single document called Prompts.md which lists
1. Every single prompt I have given in this thread, this project
2. The model used to reply, and how long the agent took to work out a reply. (Don't list the complete answer).
```

