# geolook

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aigclink/geolook, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/geolook

## Pinned environment

- Project commit: `9492cb3a1952f1370cca0f66715f87165fd56e2c`
- Test commit: `9492cb3a1952f1370cca0f66715f87165fd56e2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 2.9 | 1 | 1 | [run](https://argusic.com/run/188f38de-5cef-4ba3-b4e9-d68feb47aabf) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Python (3.12) externally managed , pip install of requests/bs4/lxml blocked`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
