# HASmartThermostat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ScratMan/HASmartThermostat, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/hasmartthermostat

## Pinned environment

- Project commit: `ef52b37fd981a3c45056c09b2593df55cc195db6`
- Test commit: `ef52b37fd981a3c45056c09b2593df55cc195db6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.7 to 39.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 39.7 | 4 | 4 | [run](https://argusic.com/run/43e36da9-27f9-4e15-ae1b-e32f165a6695) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip3 install homeassistant failed: externally-managed-environment (PEP 668); system Python cannot be written to`
- 1 min: `hass rejected the flag --log-print yes (README-era, removed from the 2025.1.4 CLI)`
- 2 min: `configuration.yaml validation: 'switch' is an invalid option for 'template' in this HA version`
- 2 min: `Mock heater turn_on failed because Action notify.persistent_notification was not found (notify integration not loaded)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
