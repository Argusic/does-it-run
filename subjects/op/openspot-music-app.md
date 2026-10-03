# openspot-music-app

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BlackHatDevX/openspot-music-app, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openspot-music-app

## Pinned environment

- Project commit: `640af8290f7deafc147143c12fbb0e12e11ba536`
- Test commit: `640af8290f7deafc147143c12fbb0e12e11ba536`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.8 to 20.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 4.8 | 0 | 0 | [run](https://argusic.com/run/b8a4162f-d6b3-49b6-9b9c-29e4e10e906c) |
| 2 | pass | 100 | 15 | 20.3 | 3 | 3 | [run](https://argusic.com/run/e1735aac-54f3-463d-89c2-dae66bdcb71d) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Missing expo-asset dependency caused web export to fail`
- 2 min: `Missing query-string dependency required by expo-router`
- 2 min: `Missing shaka-player dependency required by react-native-track-player`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
