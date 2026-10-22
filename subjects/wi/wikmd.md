# wikmd

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Linbreux/wikmd, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/wikmd

## Pinned environment

- Project commit: `5759d5192801a0639ca1b05c4260642ed4b2de6b`
- Test commit: `5759d5192801a0639ca1b05c4260642ed4b2de6b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 1.9 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 1.9 | 0 | 0 | [run](https://argusic.com/run/a20d7392-0e7c-4daf-aefe-d1f7f719b862) |
| 2 | pass | 100 | 0.15 | 13.8 | 1 | 1 | [run](https://argusic.com/run/c2a6500d-bc22-4eff-b08e-39085a1c7909) |

## What was observed on a clean machine

Attempt 2:

- 10 min: `test_watchdog and test_watchdog_subdirectory flaky: multiprocessing.Process-based Observer not ready before files created`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
