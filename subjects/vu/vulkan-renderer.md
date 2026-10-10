# vulkan-renderer

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/inexorgame/vulkan-renderer, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/vulkan-renderer

## Pinned environment

- Project commit: `ac0b20fd80b987b3cdf567143147bc2fd054751d`
- Test commit: `ac0b20fd80b987b3cdf567143147bc2fd054751d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 47.2 to 47.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 38 | 47.2 | 3 | 3 | [run](https://argusic.com/run/00fc9c9c-c5b9-4a9d-9d8c-46f77a558510) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `Missing build deps (X11/Wayland/GL dev headers, glslangValidator, Vulkan ICD) in base container; configured via userland .deb sysroot with GLFW_BUILD_WAYLAND=OFF`
- 12 min: `Example app segfaulted on startup: base destructor dereferenced uninitialized m_device whenever construction failed early (no X/GLFW connection), and CLI11 --help/--version auto-exit raced async spdlog teardown`
- `Test suite has 2 pre-existing failures identical on upstream main (Swapchain.choose_image_extent checks unset caps.currentExtent; CubeCollision.CollisionCheck divides by zero for axis-aligned ray)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
