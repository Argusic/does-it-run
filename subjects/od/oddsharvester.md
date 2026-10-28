# OddsHarvester

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jordantete/OddsHarvester, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/oddsharvester

## Pinned environment

- Project commit: `ab8c32d3c0f00db71f885ad0b30116fd723bab30`
- Test commit: `ab8c32d3c0f00db71f885ad0b30116fd723bab30`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.8 to 39.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 39.8 | 1 | 1 | [run](https://argusic.com/run/b2773f67-c688-4438-8edf-48403ab2715b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `uv binary not on subprocess PATH (installed to ~/.local/bin)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
