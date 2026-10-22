# flock

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/duckbugio/flock, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/flock

## Pinned environment

- Project commit: `d933e6a6b09f4ef4f023857c1518131ab673f081`
- Test commit: `d933e6a6b09f4ef4f023857c1518131ab673f081`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 6.6 | 1 | 1 | [run](https://argusic.com/run/93ad5f67-165e-48fa-aafb-e4c5a7b1fce1) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.26.6 not installed on system (no root for apt install)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
