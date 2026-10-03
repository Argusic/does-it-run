# Overload

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Overload-Technologies/Overload, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/overload

## Pinned environment

- Project commit: `d013cf05a90b033f1a02604aedc39d84050662ff`
- Test commit: `d013cf05a90b033f1a02604aedc39d84050662ff`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 16.6 to 18.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 17 | 16.6 | 6 | 6 | [run](https://argusic.com/run/ab549a28-7677-4b41-8451-624b294f03bb) |
| 2 | pass with mocks | 92 | 15 | 18.2 | 9 | 9 | [run](https://argusic.com/run/d465b54b-265b-46bc-9ee0-d6b75e8f03df) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `clang not found (premake5.lua defaults to clang on Linux)`
- 1 min: `Missing GL/gl.h header required by GLFW`
- 5 min: `Missing X11/Xlib.h, X11/extensions/Xrandr.h, X11/Xcursor/Xcursor.h, X11/extensions/Xrender.h, X11/extensions/Xinerama.h headers`
- 1 min: `ignored-attributes warning treated as error in OvWindowing Makefile`
- 2 min: `Missing -lGL and -lX11 linker symlinks`
- 1 min: `zenity not installed (required by OvEditor)`

Attempt 2:

- 1 min: `clang++: not found , premake5 Lua generates Makefiles that invoke clang/clang++ by default on Linux`
- 3 min: `GL/gl.h: No such file or directory , missing OpenGL development headers`
- 1 min: `KHR/khrplatform.h: No such file or directory`
- 5 min: `X11/Xlib.h: No such file or directory , missing X11 development headers`
- 1 min: `X11/extensions/Xrender.h: No such file or directory , cascading X11 header dependency`
- 1 min: `X11/extensions/Xfixes.h: No such file or directory`
- 1 min: `Werror=ignored-attributes , GCC 13 treats decltype(&pclose) in unique_ptr as warning/error`
- 2 min: `cannot find -lGL, cannot find -lX11 , linker missing .so symlinks for libGL and libX11`
- 1 min: `zenity: required by OvEditor on Linux, not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
