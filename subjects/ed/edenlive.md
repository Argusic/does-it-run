# EdenLive

**Verdict: runs with mocks.** Argusic Score 84 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/VAST-AI-Research/EdenLive, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/edenlive

## Pinned environment

- Project commit: `0b78d211bfa87b6d9b6281e9e36e55b974fe7bec`
- Test commit: `0b78d211bfa87b6d9b6281e9e36e55b974fe7bec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.9 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 84 | 28 | 12.9 | 5 | 3 | [run](https://argusic.com/run/4507c9b1-13cc-494f-89ab-b11d0b874d9d) |

## What was observed on a clean machine

Attempt 1:

- `No CUDA GPU available; offline inference requires NVIDIA GPU`
- 2 min: `Missing triton module for flashdreams attention kernels`
- 1 min: `numpy 2.5.4 incompatible with flashdreams (<2.5 required)`
- `Missing playwright module for game rendering and cover capture tests`
- `decord 0.6.0 not supported on this platform (pip check warning)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
