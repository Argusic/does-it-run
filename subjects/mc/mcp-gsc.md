# mcp-gsc

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AminForou/mcp-gsc, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-gsc

## Pinned environment

- Project commit: `d49eea9e5efb5eb645b722249303179b2c150b49`
- Test commit: `d49eea9e5efb5eb645b722249303179b2c150b49`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 1.9 to 2.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 2.7 | 0 | 0 | [run](https://argusic.com/run/4be98a0f-e887-4bd7-9a88-56346355fd06) |
| 2 | pass | 100 | 2 | 1.9 | 2 | 2 | [run](https://argusic.com/run/7092ffc7-30c0-4337-9d10-3efa61bbb6d0) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Externally managed Python environment prevented system pip install`
- 1 min: `pytest not installed in venv`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
