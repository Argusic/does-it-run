# corona

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coronalabs/corona, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/corona

## Pinned environment

- Project commit: `b45ff4b35166e0b182bb1503e27c085ad6dc0476`
- Test commit: `b45ff4b35166e0b182bb1503e27c085ad6dc0476`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 48 to 48 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 45 | 48 | 9 | 9 | [run](https://argusic.com/run/ec20d2a4-5c1e-4195-a17d-aca2640442c0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing zlib1g-dev headers`
- 8 min: `Missing OpenGL headers and libraries (GL/gl.h, libGL.so, libGLX.so)`
- 1 min: `Missing OpenAL headers`
- 1 min: `Missing Freetype headers`
- 1 min: `Missing PNG headers`
- 5 min: `Missing CURL headers (curl/curl.h)`
- 8 min: `Missing SDL2 headers (SDL.h, SDL2/SDL.h)`
- 3 min: `Missing JPEG headers (jpeglib.h, jconfig.h)`
- 5 min: `Linker could not find -lGL, -lz, -lopenal, -lfreetype, -lpng, -ljpeg, -lcurl, -lSDL2`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
