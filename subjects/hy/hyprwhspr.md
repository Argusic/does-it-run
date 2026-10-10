# hyprwhspr

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/goodroot/hyprwhspr, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/hyprwhspr

## Pinned environment

- Project commit: `07b2da36d11e4409850e07df8d4008323dd4d69e`
- Test commit: `07b2da36d11e4409850e07df8d4008323dd4d69e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.7 to 16.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 16.7 | 3 | 3 | [run](https://argusic.com/run/b41342eb-e9e9-4adc-9c4f-8c6b2a9dc77a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `externally-managed-environment blocks system pip`
- 6 min: `evdev C extension build fails: Python.h not found`
- 1 min: `CLI launcher (bin/hyprwhspr) requires system Python with distro packages; venv Python lacks rich via /usr/bin/python3`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
