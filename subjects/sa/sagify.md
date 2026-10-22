# sagify

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Kenza-AI/sagify, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/sagify

## Pinned environment

- Project commit: `054a6a2edc215db8a0b84b7e7564d076115fc43d`
- Test commit: `054a6a2edc215db8a0b84b7e7564d076115fc43d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14.3 to 14.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 30 | 14.3 | 3 | 3 | [run](https://argusic.com/run/7d697771-0677-493d-8466-abf1b750532c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `future 0.18.3 references removed 'imp' module on Python 3.12`
- 3 min: `pkg_resources missing with setuptools 84.x`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
