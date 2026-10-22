# ha-solarman

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/davidrapan/ha-solarman, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ha-solarman

## Pinned environment

- Project commit: `ac1d88b83268beeb0511b8a1b7fc8e17deddc044`
- Test commit: `ac1d88b83268beeb0511b8a1b7fc8e17deddc044`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 0.2 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 2.5 | 7.1 | 2 | 2 | [run](https://argusic.com/run/e5ee3275-aa51-49a2-a357-ba5682bc2100) |
| 2 | fail | 20 | n/a | 0.2 | 0 | 0 | [run](https://argusic.com/run/03ce90d4-1ba0-4899-bb35-c0ba7e021fd9) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Missing homeassistant.helpers.service_info.dhcp module (DhcpServiceInfo moved in HA 2025.2.0 which requires Python 3.13)`
- 0.3 min: `netifaces build fails (missing Python.h header) - only needed by tools/discovery_reply.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
