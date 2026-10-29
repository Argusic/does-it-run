# TheHive4py

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TheHive-Project/TheHive4py, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/thehive4py

## Pinned environment

- Project commit: `6a4765c39a65c328032343923de866ab4ad10127`
- Test commit: `6a4765c39a65c328032343923de866ab4ad10127`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 5.2 | 3 | 3 | [run](https://argusic.com/run/09054fae-541c-4c91-bfe2-1e52cdb11df9) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install failed due to externally-managed-environment`
- 0.3 min: `Docker not available: integration tests require a live TheHive container`
- 0.1 min: `test_init.py fixture requires Docker (session-scoped container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
