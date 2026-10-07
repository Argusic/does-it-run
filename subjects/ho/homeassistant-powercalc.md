# homeassistant-powercalc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bramstroker/homeassistant-powercalc, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/homeassistant-powercalc

## Pinned environment

- Project commit: `80c16afc0f7fc0b75e4e1fa781709de4e4ad84a3`
- Test commit: `80c16afc0f7fc0b75e4e1fa781709de4e4ad84a3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.1 | 1 | 1 | [run](https://argusic.com/run/61bbb386-cad4-4cf3-a513-ad7aa294c5ec) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `ModuleNotFoundError: No module named 'custom_components.test'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
