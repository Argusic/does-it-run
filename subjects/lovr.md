# lovr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bjornbytes/lovr, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/lovr

## Pinned environment

- Project commit: `88fa3d43698fd986f275d16956871e38111e0fca`
- Test commit: `88fa3d43698fd986f275d16956871e38111e0fca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.5 to 23.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 23.5 | 8 | 8 | [run](https://argusic.com/run/bb0278a3-35ad-4d8f-a316-21d446187fa6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `X11 development headers not installed in container`
- 2 min: `Missing nested git submodules (phonon deps, enet)`
- 2 min: `CMake couldn't find X11 headers/libs`
- 1 min: `Missing zlib1g-dev for phonon/submodule zlib`
- 1 min: `Runtime missing shared libraries (libglfw, libluajit, etc.)`
- 2 min: `Vulkan driver not available (vkCreateInstance failed)`
- 1 min: `lovr-http plugin failed: curl/curl.h not found`
- `Audio module fails to init: No backend`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
