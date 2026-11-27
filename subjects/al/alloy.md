# alloy

**Verdict: runs.** Argusic Score 53.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/grafana/alloy, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/alloy

## Pinned environment

- Project commit: `389e3d59e9c73ade9f91b72f35353267ded3dc29`
- Test commit: `389e3d59e9c73ade9f91b72f35353267ded3dc29`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 61.1 to 69.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 61.1 | 0 | 0 | [run](https://argusic.com/run/f57ccb17-cdc7-41b1-9178-df52e3274ca8) |
| 2 | pass | 86.67 | 2 | 69.7 | 3 | 1 | [run](https://argusic.com/run/720ee25b-c5b8-4b73-9733-feb784e8f5cb) |

## What was observed on a clean machine

Attempt 2:

- `libsystemd-dev not available - no root to install system packages`
- `make test: alloycli test OOM-killed during parallel run (signal: killed from Go linker)`
- `make lint requires mise+task toolchain, which can't be installed due to noexec on overlay filesystem`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
