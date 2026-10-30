# NovelRT

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/novelrt/NovelRT, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/novelrt

## Pinned environment

- Project commit: `7b23d9d5f66d3d19003504d89d576169893dc44f`
- Test commit: `7b23d9d5f66d3d19003504d89d576169893dc44f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.1 to 21.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 21.1 | 6 | 6 | [run](https://argusic.com/run/1e9daf53-1341-417e-8ced-63ed42b42597) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing X11 development headers (libx11-dev, x11proto-dev, libxcb-*-dev, etc.)`
- 1 min: `Missing wayland-scanner binary`
- 3 min: `Missing Vulkan development headers (libvulkan-dev only provided v1.3.275, code requires v1.4+ for VK_KHR_MAINTENANCE_7)`
- 1 min: `CMake 3.28 too old for cmake_policy(VERSION 3.29..3.31) in NovelRTBuildSystem.cmake`
- 6 min: `GCC compilation errors: -Wabi warns about nothing, unused variables, extra semicolons, -Wconversion errors`
- `Samples abort at runtime due to missing Vulkan GPU driver`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
