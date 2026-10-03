# bevy

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bevyengine/bevy, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/bevy

## Pinned environment

- Project commit: `cfeaeda7bff117ea1b36018c99e382455243e603`
- Test commit: `cfeaeda7bff117ea1b36018c99e382455243e603`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 38.8 to 79.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 79.8 | 0 | 0 | [run](https://argusic.com/run/84ee4d7b-cee1-4aaa-8c1c-cb05021497df) |
| 2 | pass | 100 | 5 | 38.8 | 5 | 5 | [run](https://argusic.com/run/683f08a0-8c81-43d2-86ca-3841d9bb09e3) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `wayland-sys build failed: pkg-config could not find wayland-client.pc (missing libwayland-dev)`
- 1 min: `Linker failed: unable to find -lwayland-client (no .so symlinks for the dev libraries)`
- 1 min: `winit compilation error: 'The platform you are compiling for is not supported by winit' (neither x11 nor wayland features enabled)`
- 1 min: `headless example panicked: 'ScheduleRunnerPlugin does not exist in this PluginGroup'`
- 2 min: `16 bevy_ecs should_panic tests failed when debug feature was not enabled (expected parameter names but got error codes)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
