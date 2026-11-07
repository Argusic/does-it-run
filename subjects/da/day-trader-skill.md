# day-trader-skill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jakeschincariol/day-trader-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/day-trader-skill

## Pinned environment

- Project commit: `3d0f4ef6986f4984b7c6bd46f7ff4f87744c3abd`
- Test commit: `3d0f4ef6986f4984b7c6bd46f7ff4f87744c3abd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.6 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.7 | 0 | 0 | [run](https://argusic.com/run/e60bc80e-cd5e-4b3c-bff3-6d5e3d0347db) |
| 2 | pass | 100 | 0 | 1.6 | 1 | 1 | [run](https://argusic.com/run/1d0a070a-fa60-43f1-8852-4b673e1fc237) |

## What was observed on a clean machine

Attempt 2:

- `test_repo.py fails when run directly due to _load module not on PYTHONPATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
