# hex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/anomalyco/hex, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/hex

## Pinned environment

- Project commit: `279215a5532cc1dc24abf148302a3b93132433c5`
- Test commit: `279215a5532cc1dc24abf148302a3b93132433c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28.5 to 28.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 36 | 28.5 | 3 | 3 | [run](https://argusic.com/run/4d08702e-5e14-4bad-8a6a-1fd11afbc5ba) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `Missing system dev libraries (glib, gtk, x11, xcb, alsa, vulkan, etc.) - no root access for apt install`
- 5 min: `transcribe-cpp-sys CMake build failed: Could NOT find Vulkan (missing Vulkan_LIBRARY, Vulkan_INCLUDE_DIR, glslc, SPIRV-Headers)`
- 3 min: `rust-lld linker: unable to find libraries (pangocairo, vulkan, openblas, z, xcb) and undefined symbols in static libxcb.a`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
