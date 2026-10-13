# switchfin

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dragonflylee/switchfin, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/switchfin

## Pinned environment

- Project commit: `ee04d1d465a25d87ef81c8a87a6f46f5e2541db4`
- Test commit: `ee04d1d465a25d87ef81c8a87a6f46f5e2541db4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 30.1 to 33.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 30 | 33.6 | 7 | 7 | [run](https://argusic.com/run/1f3be69a-faf5-401a-8e36-541b333f0e57) |
| 2 | pass | 100 | 25 | 30.1 | 6 | 6 | [run](https://argusic.com/run/7596f2fd-36df-4612-b163-34b4a8983ac8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Git submodules not initialized - borealis and lunasvg empty`
- 12 min: `Missing dev headers for curl/webp/mpv/glfw/x11/xcb/ffmpeg/dbus/wayland/xrandr etc.`
- 3 min: `CMake SDL2 build failed due to missing libxext-dev + X.h`
- 2 min: `CMake DBUS_ARCH_INCLUDE_DIR and DBUS_LIBRARIES not found`
- 1 min: `mpv_core.cpp unconditionally defines GLFW_EXPOSE_NATIVE_WAYLAND on Linux`
- 4 min: `LD undefined refs to libdvdnav/libmujs/liblua5.2/libsixel/libXpresent/libva-wayland`
- 1 min: `App crashed at launch: D-Bus not initialized`

Attempt 2:

- 3 min: `Missing wayland-scanner (GLFW build dep)`
- 4 min: `Missing X11 headers/xkb (GLFW X11)`
- 3 min: `FindCURL/FindMPV/FindDBus could not locate headers/libs in local prefix`
- 2 min: `wayland-client.h missing for app's GLFW_EXPOSE_NATIVE_WAYLAND`
- 12 min: `Link errors: undefined symbols from static libavformat/libavcodec and transitive libmpv deps`
- 2 min: `App aborted at startup: dbus_bus_name_has_owner assertion (no session bus in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
