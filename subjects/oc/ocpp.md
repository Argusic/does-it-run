# ocpp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lbbrhzn/ocpp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ocpp

## Pinned environment

- Project commit: `e4f7306232d2ccb41ddd54b007fbda94d96b2560`
- Test commit: `e4f7306232d2ccb41ddd54b007fbda94d96b2560`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 55 to 55 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 55 | 55 | 6 | 6 | [run](https://argusic.com/run/e4fdf178-778f-4fea-bc5d-f11f4b221744) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 external environment blocks system pip`
- 3 min: `pytest-homeassistant-custom-component==0.13.365 requires Python >=3.14, only Python 3.12 available`
- 5 min: `DeviceRegistry.async_get_devices() missing in HA 2025.x`
- 1 min: `template._parse_result() not available in HA 2025.x`
- 2 min: `_async_abort_entries_match matches the entry being reconfigured in HA 2025.x`
- 1 min: `timeout marker missing from setup.cfg strict-markers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
