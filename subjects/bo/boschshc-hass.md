# boschshc-hass

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tschamm/boschshc-hass, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/boschshc-hass

## Pinned environment

- Project commit: `dee60155deb107fef16dd6c2813681b6e2931a40`
- Test commit: `dee60155deb107fef16dd6c2813681b6e2931a40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 24.2 to 24.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 24.2 | 4 | 4 | [run](https://argusic.com/run/4be2fac9-ffc5-452b-921d-7fdfd28232eb) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `HA 2026.9.2+ required Python 3.14.2+, only Python 3.12 available; installed HA 2025.1.4 as fallback which works for most tests`
- 2 min: `ZeroconfServiceInfo import path differs between HA versions (helpers.service_info.zeroconf vs components.zeroconf)`
- 2 min: `OptionsFlowWithReload not available in HA 2025.1.4, replaced by OptionsFlowWithConfigEntry`
- 1 min: `Harness tests incompatible with installed HA 2025.1.4 (require HA beta matching phccc version)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
