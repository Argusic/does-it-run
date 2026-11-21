# StreamRAG

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/video-db/StreamRAG, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/streamrag

## Pinned environment

- Project commit: `f785ddbdc5d677dc7d586d421451e7b32b46c2c2`
- Test commit: `f785ddbdc5d677dc7d586d421451e7b32b46c2c2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 3.3 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 3.4 | 0 | 0 | [run](https://argusic.com/run/4361fc2b-2add-40f2-ba5d-ae027ca8079e) |
| 2 | pass with mocks | 92 | 1 | 3.3 | 2 | 2 | [run](https://argusic.com/run/5110da5c-6faa-46b0-8f49-345eb926ecf3) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pip install fails: externally-managed-environment (PEP 668)`
- 2 min: `app.py get_connection() hardcoded connect() with no way to mock base_url`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
