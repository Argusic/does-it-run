# exo

**Verdict: runs.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/exo-explore/exo, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/exo

## Pinned environment

- Project commit: `21a54c5ea0230a3bec1e1a786d200126c7e34ec6`
- Test commit: `21a54c5ea0230a3bec1e1a786d200126c7e34ec6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.6 to 15.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 92 | 10 | 15.6 | 5 | 3 | [run](https://argusic.com/run/bea1a92c-b857-44a4-bbd8-756185dbd0e7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv binary not found in environment`
- 1 min: `Python 3.13 not available (system has 3.12)`
- 1 min: `exo_tools workspace package not installed by uv sync`
- `mlx.core CUDA prebuilt wheel has undefined symbol on CPU-only Linux container`
- `5 test collection errors in mlx/worker tests due to missing GPU accelerator`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
