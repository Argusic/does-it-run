# nCine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nCine/nCine, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/ncine

## Pinned environment

- Project commit: `e9a2342262e193d2343e69989b6f73cb8ba2cf10`
- Test commit: `e9a2342262e193d2343e69989b6f73cb8ba2cf10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 11.7 | 5 | 5 | [run](https://argusic.com/run/4d2c2643-51a2-47ff-922a-fe62aa3a6717) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `OpenGL not found - missing GL dev headers and lib symlinks`
- 2 min: `SDL2 dev headers not found (runtime was installed but no -dev package)`
- 1 min: `GL/glext.h and KHR/khrplatform.h not found from minimal fake GL header`
- 1 min: `Debian SDL_config.h uses arch-specific include <SDL2/_real_SDL_config.h>`
- 1 min: `Sdl2InputManager.cpp failed with incomplete SDL types`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
