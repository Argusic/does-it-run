# industrial_ci

**Verdict: runs with mocks.** Argusic Score 76 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ros-industrial/industrial_ci, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/industrial-ci

## Pinned environment

- Project commit: `125164b9f1883cdf1858897a7146d1bebf2be5c6`
- Test commit: `125164b9f1883cdf1858897a7146d1bebf2be5c6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 7.6 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3.5 | 7.6 | 0 | 0 | [run](https://argusic.com/run/0faeb578-d8fb-448a-a710-b9f4dc76cd29) |
| 2 | pass with mocks | 72 | 9 | 9.9 | 3 | 0 | [run](https://argusic.com/run/e5be7e00-19b2-443e-8cad-90bd42efd965) |

## What was observed on a clean machine

Attempt 2:

- `Docker not installed - run_travis job execution requires docker to pull ROS images`
- `No root/sudo access - isolation=shell fails at apt-get update/lock`
- `No local Python test suite - 0 tests found in industrial_ci package`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
