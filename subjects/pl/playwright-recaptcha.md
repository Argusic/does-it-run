# Playwright-reCAPTCHA

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Xewdy444/Playwright-reCAPTCHA, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/playwright-recaptcha

## Pinned environment

- Project commit: `086d8407c0eb22a60ce50201d53e4298b90d492d`
- Test commit: `086d8407c0eb22a60ce50201d53e4298b90d492d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 6.7 | 1 | 1 | [run](https://argusic.com/run/fbbbd408-9783-4961-84c1-9e18b4a90a96) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `AsyncSolver.solve_recaptcha passed a sync lambda to AsyncRetrying, which returns a coroutine object instead of awaiting it; causes AttributeError on line 633`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
