# solaredge-modbus-multi

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WillCodeForCats/solaredge-modbus-multi, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/solaredge-modbus-multi

## Pinned environment

- Project commit: `d38d890887684ddd7938c4bce5223d387b24c6a7`
- Test commit: `d38d890887684ddd7938c4bce5223d387b24c6a7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.7 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 8.7 | 4 | 4 | [run](https://argusic.com/run/8c945cf8-9e18-48ef-9f7c-4d2b72cc08e7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `requirements-test.txt has conflicting pytest pin (pytest>=8.0.0 conflicts with pytest-homeassistant-custom-component's pinned pytest==8.3.4)`
- 2 min: `Missing UnitOfReactiveEnergy and SensorDeviceClass.REACTIVE_ENERGY in HA 2025.1.4 (shipped by test harness)`
- 1 min: `ZeroconfServiceInfo not found in helpers.service_info.zeroconf in HA 2025.1.4 (was in components.zeroconf)`
- 1 min: `Missing zeroconf package (required by fallback import path)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
