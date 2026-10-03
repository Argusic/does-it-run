# supertux

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SuperTux/supertux, licensed GPL-3.0, written in C++.

Evidence and recordings: https://argusic.com/subject/supertux

## Pinned environment

- Project commit: `7852251d827f576fcc918c2a8d23c781bc28b2ad`
- Test commit: `7852251d827f576fcc918c2a8d23c781bc28b2ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 27.1 to 28.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 28.8 | 5 | 5 | [run](https://argusic.com/run/611cb9e9-f343-4119-a8ee-17f7dfda0f30) |
| 2 | fail | 20 | n/a | 27.1 | 0 | 0 | [run](https://argusic.com/run/96483e6d-737e-4a0e-b85c-4a12e863d1df) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Missing system development packages (SDL3, libpng, zlib, freetype, fmt, glm, physfs, openal, glew, libcurl, libogg, libvorbis)`
- 1 min: `SDL3_ttf required SDL3 >= 3.2.6 but built SDL3 was 3.2.4`
- 1 min: `GLEW build failed due to missing OpenGL headers and auto-generated sources`
- 0.5 min: `SDL3_image pkg-config file not installed after build`
- 0.5 min: `glm cmake config had broken relative path for include dirs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
