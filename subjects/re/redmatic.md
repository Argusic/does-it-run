# RedMatic

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rdmtc/RedMatic, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/redmatic

## Pinned environment

- Project commit: `dfc15b3b640b6f88d83c6ca3cf12d157c3c91be2`
- Test commit: `dfc15b3b640b6f88d83c6ca3cf12d157c3c91be2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 3.6 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 6.1 | 0 | 0 | [run](https://argusic.com/run/88ba3624-946a-4d3e-90cb-2d7e5f23acc9) |
| 2 | pass | 100 | 0.5 | 3.6 | 2 | 2 | [run](https://argusic.com/run/cbdc7c6d-4159-42ec-b173-4ba3c3cf03c0) |

## What was observed on a clean machine

Attempt 2:

- 0.3 min: `patchelf binary not pre-installed in container`
- `engine warnings during npm install (host node v18 but packages target >=22)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
