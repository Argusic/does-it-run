# vulkan-renderer

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/inexorgame/vulkan-renderer, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/vulkan-renderer

## Pinned environment

- Project commit: `ac0b20fd80b987b3cdf567143147bc2fd054751d`
- Test commit: `ac0b20fd80b987b3cdf567143147bc2fd054751d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 21 to 47.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 38 | 47.2 | 3 | 3 | [run](https://argusic.com/run/00fc9c9c-c5b9-4a9d-9d8c-46f77a558510) |
| 2 | pass | 100 | 21 | 21 | 6 | 6 | [run](https://argusic.com/run/c42c64e2-c365-4353-86e7-5b6bf7836cc3) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `Missing build deps (X11/Wayland/GL dev headers, glslangValidator, Vulkan ICD) in base container; configured via userland .deb sysroot with GLFW_BUILD_WAYLAND=OFF`
- 12 min: `Example app segfaulted on startup: base destructor dereferenced uninitialized m_device whenever construction failed early (no X/GLFW connection), and CLI11 --help/--version auto-exit raced async spdlog teardown`
- `Test suite has 2 pre-existing failures identical on upstream main (Swapchain.choose_image_extent checks unset caps.currentExtent; CubeCollision.CollisionCheck divides by zero for axis-aligned ray)`

Attempt 2:

- 2 min: `glslangValidator (shader compiler) not found on system`
- 1 min: `GLFW required Wayland but wayland-scanner not present on system`
- 5 min: `X11 development headers (X11/Xlib.h, X11/X.h etc.) missing from container`
- 3 min: `FindX11 failed to locate XKB headers (X11/extensions/XKB.h)`
- 1 min: `GL/gl.h not found when compiling against glfw3.h`
- 4 min: `Numerous xcb extension headers and libs missing (xcb/randr.h, composite.h, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
