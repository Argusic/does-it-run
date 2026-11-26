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
- Valid runs: 2; wall time 12 to 13.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 12 | 3 | 3 | [run](https://argusic.com/run/7aea1d0b-8722-493b-b1ef-7de5665a9a4a) |
| 2 | pass with mocks | 92 | 2 | 13.3 | 6 | 6 | [run](https://argusic.com/run/356d0166-d3d7-4a3e-9f7d-52766a10be9c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Python 3.13 required by Makefile but only 3.12 available in the container`
- 3 min: `ModuleNotFoundError: No module named 'aiofiles' during test import`
- 5 min: `Thread cleanup assertion: pycares creates a daemon thread '_run_safe_shutdown_loop' that pytest-homeassistant-custom-component's verify_cleanup fixture rejects`

Attempt 2:

- 3 min: `homeassistant>=2026.6.4 requires Python 3.13; container has Python 3.12.3`
- 2 min: `test_keyless_weather_setup.py teardown: _run_safe_shutdown_loop thread check assertion in pytest-homeassistant-custom-component`
- 2 min: `50 component unit tests fail (HA 2026 API shape mismatch) and 19 error on teardown`
- 2 min: `test_comprehensive.py errors: Mock async methods not properly awaited (SmartIrrigationCoordinator constructor triggers await on mocked store)`
- 1 min: `test_enhanced_scheduling.py: 8 failures due to missing _save_schedules method (unimplemented feature)`
- 1 min: `test_weather_records_proof.py: ImportError from relative import in websockets.py when run as script`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
