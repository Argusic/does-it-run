# HomeAssistant-Tapo-Control

**Verdict: could not verify.** Argusic Score 77.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JurajNyiri/HomeAssistant-Tapo-Control, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/homeassistant-tapo-control

## Pinned environment

- Project commit: `1b7a7d6fa671047d04c092fee4f0e7bed1b8ee58`
- Test commit: `1b7a7d6fa671047d04c092fee4f0e7bed1b8ee58`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 8.7 to 11.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 9 | 8.7 | 5 | 5 | [run](https://argusic.com/run/44713155-8539-42c0-ab82-d6355a245a58) |
| 2 | fail | 75 | 10.2 | 11.2 | 8 | 6 | [run](https://argusic.com/run/a5564864-22ae-4c27-a929-f495ce290ae6) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `externally-managed-environment preventing system pip install`
- 1 min: `haffmpeg package not found (pip install haffmpeg fails)`
- 2 min: `onvif-zeep-async 4.3.0 requires aiohttp>=3.12.9 but HA 2025.1.4 needs aiohttp==3.11.11`
- 1 min: `Missing Python packages: aiofiles, numpy`
- `Manifest requires HA 2026.9.0 but installed HA is 2025.1.4`

Attempt 2:

- 0.3 min: `Externally-managed Python environment prevents system pip install`
- 0.5 min: `Missing haffmpeg module (required by HA ffmpeg component)`
- 4 min: `Missing onvif module (required by tapo_control utils.py)`
- 0.5 min: `Missing onvif.util submodule (required by HA onvif component)`
- 0.8 min: `Missing aiofiles module (required by pytapo)`
- 3.5 min: `Missing numpy module (required by HA stream component)`
- 1 min: `WSDiscovery==2.0.0 (pinned by HA onvif manifest) depends on netifaces C extension that requires python3-dev headers (no root); installed WSDiscovery 2.1.2 as substitute`
- `Manifest requires homeassistant 2026.9.0 but installed version is 2025.1.4; all imports and compile check pass regardless`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
