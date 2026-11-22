# geolook

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aigclink/geolook, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/geolook

## Pinned environment

- Project commit: `9492cb3a1952f1370cca0f66715f87165fd56e2c`
- Test commit: `9492cb3a1952f1370cca0f66715f87165fd56e2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 2.9 | 1 | 1 | [run](https://argusic.com/run/188f38de-5cef-4ba3-b4e9-d68feb47aabf) |
| 2 | pass | 100 | 4 | 2.9 | 2 | 2 | [run](https://argusic.com/run/0b19bd80-5001-410e-b7a7-eb562d182a10) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Python (3.12) externally managed , pip install of requests/bs4/lxml blocked`

Attempt 2:

- 1 min: `externally-managed-environment: system pip blocked by PEP 668`
- 0.5 min: `Port 8765 already in use on second launch attempt`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
