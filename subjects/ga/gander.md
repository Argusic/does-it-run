# gander

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mokshablr/gander, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/gander

## Pinned environment

- Project commit: `60cc6e5d13b6ddaafef238e1f899b7d79a93dec4`
- Test commit: `60cc6e5d13b6ddaafef238e1f899b7d79a93dec4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 10.2 to 24.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 24.6 | 0 | 0 | [run](https://argusic.com/run/80dc4883-6a90-4c76-ac48-3d065b1af645) |
| 2 | pass | 100 | 10.5 | 10.2 | 5 | 5 | [run](https://argusic.com/run/4a3e65f4-7fae-4750-8505-fb0c6abd19cd) |

## What was observed on a clean machine

Attempt 2:

- 1.5 min: `No JDK installed in container`
- 3.5 min: `No Android SDK installed`
- 0.2 min: `No unzip binary available`
- 0.1 min: `sdkmanager had no execute permission`
- 0.5 min: `Package name build-tools;36 did not exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
