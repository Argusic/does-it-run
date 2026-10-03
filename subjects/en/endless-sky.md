# endless-sky

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/endless-sky/endless-sky, licensed GPL-3.0, written in C++.

Evidence and recordings: https://argusic.com/subject/endless-sky

## Pinned environment

- Project commit: `129f3ac56eafb4e437ba70c2a5e0fbfa7a057322`
- Test commit: `129f3ac56eafb4e437ba70c2a5e0fbfa7a057322`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 4; wall time 14.8 to 58.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 52.9 | 0 | 0 | [run](https://argusic.com/run/a6d932c7-7742-43b4-9d15-0bf9d64ed014) |
| 1 | fail | 80 | 51 | 58.9 | 7 | 7 | [run](https://argusic.com/run/b351934a-bc96-4655-a40b-8c23671974e5) |
| 2 | timeout | none | 42 | 46.5 | 2 | 2 | [run](https://argusic.com/run/174fd8a2-d2ff-42e2-ba6f-7cad52dcec50) |
| 2 | fail | 20 | n/a | 14.8 | 0 | 0 | [run](https://argusic.com/run/7b4dd308-911e-4d54-b68a-0c6f95422742) |

## What was observed on a clean machine

Attempt 1:

- 30 min: `No development packages (headers/libs) available on bare container - library debs had to be downloaded and staged manually`
- 5 min: `vcpkg bootstrap failed because the checked-out baseline (old commit) has schema-version 1 in vcpkg-tools.json but the bootstrapped binary expects version 2`
- 8 min: `Missing runtime .so chains for staged dev packages (libGLEW.so.2.2.0, libavif.so.16.0.4, libSDL2-2.0.so.0.3000.0, libopenal.so.1.23.1, etc.)`
- 2 min: `Missing X11/X.h header for GLX compilation`
- 3 min: `Linker errors: missing -lasound, -lpulse, -lsamplerate, X/Wayland libs from SDL2 static dependencies`
- 1 min: `libavif.so.16.0.4 needs libgav1.so.1 which needs libabsl_synchronization.so.20220623 (abseil-cpp)`
- 2 min: `libFLAC.a compiled with ogg support but -logg not linked; ambiguous symbol ogg_stream_reset`

Attempt 2:

- 40 min: `Missing system dev packages (libgl-dev, libglx-dev, libx11-dev, libsdl2-dev, libpng-dev, libjpeg-dev, libavif-dev, libglew-dev, libopenal-dev, libmad0-dev, libflac++-dev, libogg-dev, libminizip-dev, uuid-dev, zlib1g-dev, libxmu-dev, libxi-d`
- 2 min: `Missing zip/unzip utilities for vcpkg bootstrap`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
