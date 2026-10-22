# agents

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/astronomer/agents, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/run/746045ff-1fda-472c-b68d-d7383c1e9137

## Pinned environment

- Project commit: `cbe1141f547bcf0506babb9778a7696bf15eff66`
- Test commit: `cbe1141f547bcf0506babb9778a7696bf15eff66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 48.8 to 48.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 22 | 48.8 | 3 | 3 | [run](https://argusic.com/run/746045ff-1fda-472c-b68d-d7383c1e9137) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install uv blocked by PEP 668 (externally-managed-environment)`
- 8 min: `3 unit tests failed when plugin.py imported before test_server.py (plugin monkeypatched shared _manager auth getters at import time)`
- 10 min: `No Airflow instance available for integration tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
