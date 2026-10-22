# HAsmartirrigation

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/altmenorg/HAsmartirrigation, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/hasmartirrigation

## Pinned environment

- Project commit: `7d8a2d26f6ad2388858a3874d73b8612cfeb8cf6`
- Test commit: `7d8a2d26f6ad2388858a3874d73b8612cfeb8cf6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12 to 12 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 12 | 3 | 3 | [run](https://argusic.com/run/7aea1d0b-8722-493b-b1ef-7de5665a9a4a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Python 3.13 required by Makefile but only 3.12 available in the container`
- 3 min: `ModuleNotFoundError: No module named 'aiofiles' during test import`
- 5 min: `Thread cleanup assertion: pycares creates a daemon thread '_run_safe_shutdown_loop' that pytest-homeassistant-custom-component's verify_cleanup fixture rejects`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
