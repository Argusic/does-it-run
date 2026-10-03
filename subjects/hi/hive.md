# hive

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aden-hive/hive, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/hive

## Pinned environment

- Project commit: `6193aea7eb064f7536dfedcbe9ff08ad954ac53b`
- Test commit: `6193aea7eb064f7536dfedcbe9ff08ad954ac53b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.4 to 20.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 0.3 | 20.4 | 2 | 1 | [run](https://argusic.com/run/3ac0b964-30ea-408d-9fce-b293f12f10d2) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Playwright browser binaries missing`
- `test_live_health_checks.py::TestLiveIntegrationWiring::test_wiring_valid[lusha_api_key] , endpoint mismatch between spec and checker URL`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
