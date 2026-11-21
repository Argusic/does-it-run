# pmtech

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/polymonster/pmtech, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/pmtech

## Pinned environment

- Project commit: `1c4d6810836f6da2b8d9f4955aead7b9048e0b83`
- Test commit: `1c4d6810836f6da2b8d9f4955aead7b9048e0b83`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.7 to 46.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 13 | 46.4 | 5 | 4 | [run](https://argusic.com/run/5dfb3a39-dcf2-41ee-aa3f-f9628a979346) |
| 2 | pass | 100 | 13 | 15.7 | 3 | 3 | [run](https://argusic.com/run/78cce8f7-e576-4247-9435-ab260e3ff6a7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `git submodules not initialized`
- 7 min: `Linux build fails: GL/glew.h not found (no root, no dev headers)`
- 2 min: `link: cannot find -lGL (libgl1-mesa-dev ships no libs)`
- 10 min: `llvmpipe: glew glxew init needs glXGetCurrentDisplay from glXGetProcAddressARB, not provided over Xvfb, causing silent test exit`
- `cubemap test differs 2763965/3686400 pixels (74.977%) vs reference`

Attempt 2:

- 10 min: `Missing GLEW include paths and GLEW_NO_GLU define in setup_linux() premake config - os.cpp needed GL/glew.h and GL/glx.h`
- 5 min: `Missing GL/glx.h and X11/Xlib.h system headers (libgl-dev, libglx-dev, x11proto-dev packages not installed)`
- 5 min: `Missing -lGLEW, -lGLU, -lGL, -lX11 linker .so symlinks (dev packages not installed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
