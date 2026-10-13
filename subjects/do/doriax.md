# doriax

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/doriaxengine/doriax, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/doriax

## Pinned environment

- Project commit: `575ef40d0be01b24a1eae5af95a5a59d18977455`
- Test commit: `575ef40d0be01b24a1eae5af95a5a59d18977455`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 29.6 to 32.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 29.6 | 0 | 0 | [run](https://argusic.com/run/42bb1b72-cc26-4a54-bc79-5dc605e5db41) |
| 2 | pass | 100 | 32 | 32.6 | 6 | 6 | [run](https://argusic.com/run/b5ed1534-94f8-4aee-8898-f1a8884afb4c) |

## What was observed on a clean machine

Attempt 2:

- 10 min: `System lacked CURL/X11/GL/dbus/wayland dev packages and no root install possible`
- 4 min: `CMake FindX11 uses X11_X11_INCLUDE_PATH var and Xrandr needs Xrender target`
- 3 min: `wayland-scanner missing and nfd needed xdg-foreign protocol`
- 3 min: `Compiler lacked GL/curl/dbus include paths`
- 7 min: `Linker could not find libGL/libX11/libXi/libXcursor/libwayland/libdbus and static curl/dbus pulled missing gss/psl/ssh/systemd symbols`
- 3 min: `editor GUI failed at NFD_Init: /usr/bin/dbus-launch not present`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
