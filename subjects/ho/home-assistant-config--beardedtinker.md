# Home-Assistant_Config

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BeardedTinker/Home-Assistant_Config, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/707365d1-e615-402d-9a8c-f70ce43bb100

## Pinned environment

- Project commit: `3f744b323069959525584985a7e0582fcdffb844`
- Test commit: `3f744b323069959525584985a7e0582fcdffb844`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 7 | 7.5 | 4 | 3 | [run](https://argusic.com/run/707365d1-e615-402d-9a8c-f70ce43bb100) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `homeassistant==2025.12.4 requires Python >=3.13.2; only Python 3.12.3 available`
- 1 min: `service_account_ga.json missing, google_assistant.yaml load fails`
- 1 min: `secrets.yaml allow_dir: /github/workspace/tmp is inaccessible (no root)`
- `Python.h (python3-dev) missing; netifaces and pyspeex-noise wheels fail to build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
