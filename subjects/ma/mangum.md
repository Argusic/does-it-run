# mangum

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Kludex/mangum, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mangum

## Pinned environment

- Project commit: `f2adb550c7786cc23312826336e5aa7fb3a75b46`
- Test commit: `f2adb550c7786cc23312826336e5aa7fb3a75b46`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 3 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 3 | 0 | 0 | [run](https://argusic.com/run/93edb198-aaf2-431a-a62d-da22d3e2ed3f) |
| 2 | pass with mocks | 92 | 3 | 7.5 | 4 | 4 | [run](https://argusic.com/run/693789b1-088c-4d5a-9016-ba32c4c69118) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Python environment is externally managed (PEP 668), requiring venv`
- 1 min: `pip install mangum[dev] failed: dev extra not defined`
- 1 min: `boto3 and testcontainers not installed from dev extras`
- 1 min: `Docker not available: localstack fixtures crash test run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
