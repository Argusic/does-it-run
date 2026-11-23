# screen_capture_lite

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/smasherprog/screen_capture_lite, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/screen-capture-lite

## Pinned environment

- Project commit: `0c5beb0e3c5e4f9e0fcc9203025a80ad5164e6a4`
- Test commit: `0c5beb0e3c5e4f9e0fcc9203025a80ad5164e6a4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.1 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 12 | 13 | 5 | 4 | [run](https://argusic.com/run/4f879f58-52e4-4e53-80e6-046e2a8e0e2e) |
| 2 | pass | 100 | 10 | 5.1 | 2 | 2 | [run](https://argusic.com/run/d7d3683d-ebcd-45b5-bd58-a28c3ec3d513) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Could NOT find X11: libx11-dev/libxtst-dev/libxinerama-dev/libxfixes-dev absent and no root to apt-get install`
- 1 min: `X11/X.h and other core protocol headers missing from libx11-dev (split into x11proto-dev on Ubuntu 24.04)`
- 2 min: `GLFW and core lib missing XShm.h/Xrender.h/Xcursor/Xrandr/XInput headers`
- 2 min: `SCL_GetWindows hit BadAtom on bare Xvfb because no window manager sets _NET_CLIENT_LIST`
- 1 min: `C# bindings cannot build: no dotnet SDK in container`

Attempt 2:

- 7 min: `X11 development headers not installed in container (libx11-dev, libxinerama-dev, libxfixes-dev, libxtst-dev, libxrandr-dev, libxcursor-dev, libxi-dev, libxrender-dev, libxxf86vm-dev, libxext-dev, libxcb1-dev, libxcb-shm0-dev, x11proto-dev m`
- 1 min: `Static X11 .a libs not built with -fPIC, can't link into shared library`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
