# U3D

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/u3d-community/U3D, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/u3d

## Pinned environment

- Project commit: `5be027ab2759f8cc45cd8fff6af375d622550260`
- Test commit: `5be027ab2759f8cc45cd8fff6af375d622550260`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 50.9 to 50.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 50.9 | 3 | 3 | [run](https://argusic.com/run/7ad91a52-3198-439a-b720-25b2b488734f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `zlib not found: Assimp requires zlib but host has no -dev package and ASSIMP_BUILD_ZLIB defaults to OFF on Linux`
- 5 min: `X11/Xlib.h not found: GLEW needs X11 development headers for GLX support`
- 1 min: `-lGL not found: OpenGL shared library has no .so symlink`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
