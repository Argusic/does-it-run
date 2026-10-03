# cog

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/arun1729/cog, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/cog

## Pinned environment

- Project commit: `5be9863fce7e5b62fb265c85f3543fa8c0e5c527`
- Test commit: `5be9863fce7e5b62fb265c85f3543fa8c0e5c527`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.4 | 1.8 | 0 | 0 | [run](https://argusic.com/run/e50a14d6-5ced-4a18-b594-8a5b77089ab1) |
| 2 | pass | 100 | 0.2 | 2.8 | 1 | 1 | [run](https://argusic.com/run/318ce976-bb11-4d1f-909e-3e321f1ea13c) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `externally-managed-environment blocked system pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
