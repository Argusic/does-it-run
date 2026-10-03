# OpenTTD

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenTTD/OpenTTD, licensed NOASSERTION, written in C++.

Evidence and recordings: https://argusic.com/subject/openttd

## Pinned environment

- Project commit: `ed04d336ed9d78a0e9e7a517d4f40f03a3ead895`
- Test commit: `ed04d336ed9d78a0e9e7a517d4f40f03a3ead895`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 27.5 to 117 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 26 | 27.5 | 2 | 2 | [run](https://argusic.com/run/b22d537b-9471-4647-a903-983b3cf9d03f) |
| 2 | pass | 100 | 35 | 35.1 | 2 | 2 | [run](https://argusic.com/run/b42a41da-a758-4ece-85ee-7974a5820659) |
| 3 | timeout | none | n/a | 117 | 0 | 0 | [run](https://argusic.com/run/cc14ff73-c329-467e-9e2d-1227a596c24c) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Missing system -dev packages for SDL2 and related libraries (libsdl2-dev, libpng-dev, liblzma-dev, zlib1g-dev, libcurl4-openssl-dev, libfreetype-dev, libfontconfig-dev, libharfbuzz-dev, libicu-dev, liblzo2-dev, libopusfile-dev, libsoxr-dev,`
- 10 min: `GUI build failed at link stage - SDL2 cmake config pulls in dependencies for X11, Wayland, PulseAudio, libsamplerate, etc. whose -dev packages are not available. The dedicated server build succeeds.`

Attempt 2:

- 3 min: `Missing -dev packages (libsdl2-dev, zlib1g-dev, libpng-dev, liblzma-dev, libcurl-dev, libfreetype-dev, libfontconfig-dev, libharfbuzz-dev, libicu-dev) required for full desktop build`
- 1 min: `No graphics/sound/music base sets present (original TTD files require CD-ROM)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
