# pylips

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eslavnov/pylips, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pylips

## Pinned environment

- Project commit: `b6af4cc14d7e17e361f16703991b902d43d199c9`
- Test commit: `b6af4cc14d7e17e361f16703991b902d43d199c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 35.1 to 35.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 33 | 35.1 | 3 | 3 | [run](https://argusic.com/run/a079d7c6-bacc-4c2c-9291-effa1989f6ec) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip3 install -r requirements.txt blocked: externally-managed-environment (PEP 668)`
- 8 min: `is_online() crashed with FileNotFoundError: 'ping' when host unreachable (ping not installed in container)`
- 14 min: `MQTT listen mode (MQTT_update=False) crashed: AttributeError 'Pylips' object has no attribute 'last_status'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
