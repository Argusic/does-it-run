# epr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wustho/epr, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/epr

## Pinned environment

- Project commit: `305fb366ca1479e703e3b522fd5fe56b69ba31c6`
- Test commit: `305fb366ca1479e703e3b522fd5fe56b69ba31c6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.7 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 3.1 | 1 | 1 | [run](https://argusic.com/run/c4aa10b6-122f-4394-afd8-da1024d50c4a) |
| 2 | pass | 100 | 0.1 | 2.7 | 0 | 0 | [run](https://argusic.com/run/58a57940-647b-4c09-b9c8-2202f211b9f3) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Poetry install failed: cffi 1.15.1 build failed due to missing python3-dev headers and libffi`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
