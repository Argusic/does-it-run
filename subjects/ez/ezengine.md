# ezEngine

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ezEngine/ezEngine, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/ezengine

## Pinned environment

- Project commit: `4fd77fbc2bc1b35db622e6652b6be1df637c818f`
- Test commit: `4fd77fbc2bc1b35db622e6652b6be1df637c818f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 62.1 to 62.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 98 | 60 | 62.1 | 10 | 9 | [run](https://argusic.com/run/45065d08-0ef4-43b8-8a25-cbf4af7adc01) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `ninja not installed`
- 5 min: `Missing libfreetype-dev headers`
- 15 min: `Missing X11 dev headers (X11/X.h, XKBlib.h, extensions/XKB.h, extensions/Xrandr.h etc)`
- 3 min: `Missing uuid/uuid.h headers`
- 5 min: `Missing libvulkan-dev (Vulkan_INCLUDE_DIR/Vulkan_LIBRARY)`
- 3 min: `Missing GL/gl.h (GLFW dependency)`
- 2 min: `Missing libuuid.so linker symlink`
- 2 min: `Pre-existing include ordering bug: ResourceLock.h uses ezResourceManager without including it`
- 5 min: `Pre-existing Vulkan 1.3.275 API incompatibility (VK_KHR_ -> VK_EXT_ rename, swapchain maintenance features)`
- 5 min: `No root access - system packages cannot be installed, used .deb extraction workaround`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
