# ha-fordpass

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/marq24/ha-fordpass, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ha-fordpass

## Pinned environment

- Project commit: `81c08e8ef5f15f15f1e15c790bebaf1a87988b2c`
- Test commit: `81c08e8ef5f15f15f1e15c790bebaf1a87988b2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 6.4 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 10.1 | 2 | 2 | [run](https://argusic.com/run/7916bdb8-f48a-4e45-823d-f913f7f2fd4e) |
| 2 | fail | 80 | 10 | 6.4 | 0 | 0 | [run](https://argusic.com/run/e821599b-44a3-4134-85c3-0b641170e1fd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `HA 2026.9.0+ required by manifest but Python 3.12 only supports HA <= 2025.1.4 in this container`
- 1 min: `Config flow test fails: probatio SelectSelector incompatible with voluptuous in test harness`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
