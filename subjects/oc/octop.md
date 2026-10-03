# Octop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TencentCloud/Octop, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/octop

## Pinned environment

- Project commit: `e473dd3c4a4741618ffde1a42a3492341a189e8e`
- Test commit: `e473dd3c4a4741618ffde1a42a3492341a189e8e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.7 to 44.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 44.7 | 2 | 2 | [run](https://argusic.com/run/ef3b9dc0-13a5-487e-a0b2-e2228ba66aa9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv package manager not found in PATH`
- 8 min: `evdev build failure: Python.h missing (no python3-dev, no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
