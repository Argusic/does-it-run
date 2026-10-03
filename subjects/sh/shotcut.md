# shotcut

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mltframework/shotcut, licensed GPL-3.0, written in C++.

Evidence and recordings: https://argusic.com/subject/shotcut

## Pinned environment

- Project commit: `3cfd48ba16967d524e75d1197d103a246377a1a8`
- Test commit: `3cfd48ba16967d524e75d1197d103a246377a1a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 44.3 to 54.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 49.3 | 0 | 0 | [run](https://argusic.com/run/c5aa8d28-37c9-4ca2-aeb3-72fba727dc42) |
| 2 | timeout | none | 49 | 54.9 | 10 | 10 | [run](https://argusic.com/run/c2a1dcd4-6534-4dea-9b8e-356e4769b0ba) |
| 2 | pass | 100 | 61 | 44.3 | 11 | 11 | [run](https://argusic.com/run/e9869f6b-190b-4e29-887f-76faf9dd29f2) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `Qt 6.10.3 not installed`
- 10 min: `MLT 7.36.0+ not available (system had 7.22.0)`
- 3 min: `OpenGL development headers missing`
- 3 min: `XKB development headers missing`
- 3 min: `X11 development headers missing`
- 4 min: `Qt6Charts, Qt6Multimedia, and other Qt modules not installed`
- 3 min: `Vulkan headers missing`
- 3 min: `FFTW3 development headers missing`
- 1 min: `Ninja build system not available`
- 1 min: `xmldoc npm module ESM-only incompatibility`

Attempt 2:

- 1 min: `Ninja not installed in container`
- 5 min: `Qt 6.10.3 not found in ~/Qt`
- 5 min: `X11, OpenGL, GLU, FFTW, ICU, Vulkan, libxml2 dev headers missing`
- 12 min: `MLT (mlt++-7 >= 7.36.0) not found`
- 2 min: `Fix: Qt6 modules not found by cmake (WrapOpenGL missing)`
- 1 min: `Fix: XKB (libxkbcommon) not found by Qt6`
- 1 min: `Fix: X11 not found by cmake`
- 1 min: `Fix: Vulkan headers not found for hdrpreviewwindow.cpp`
- 1 min: `Fix: FFTW pkg-config prefix was /usr instead of ~/local`
- 23 min: `Build produced a 112MB debug binary`
- 2 min: `JavaScript tests (test-node.js) require manual .mlt input files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
