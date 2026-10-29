# cogent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cogentcore/cogent, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/cogent

## Pinned environment

- Project commit: `5db9d4415e5f93cb78c33c5f267be22a8cd08ab8`
- Test commit: `5db9d4415e5f93cb78c33c5f267be22a8cd08ab8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.6 to 8.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 8.6 | 4 | 4 | [run](https://argusic.com/run/a31e8151-52f0-4a20-8d71-63255ec868b0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `core setup requires sudo (sudo: command not found) to apt install system packages`
- 4 min: `GUI build failed: wayland-client-core.h (and other X11/GL dev headers) missing`
- 1 min: `link failed: cannot find -lGL (no libGL.so symlink)`
- 3 min: `marbles/settings/taskmanager panicked in WebGPU surface init: no GPU adapter available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
