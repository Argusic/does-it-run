# SubTUI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MattiaPun/SubTUI, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/subtui

## Pinned environment

- Project commit: `0d9e54bc0bb45c40044872b6b0a2598dd816c815`
- Test commit: `0d9e54bc0bb45c40044872b6b0a2598dd816c815`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 16.4 to 29.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 16.4 | 2 | 2 | [run](https://argusic.com/run/951bd0c2-1dac-45a4-a48d-f53c28267bfd) |
| 2 | pass with mocks | 92 | 30 | 29.4 | 3 | 3 | [run](https://argusic.com/run/a47cefa7-01d9-4c8b-875a-ab79b2832105) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler not installed in container`
- 5 min: `mpv player not installed in container`

Attempt 2:

- 10 min: `No Go toolchain installed in container`
- 12 min: `mpv required by README not installed (no root)`
- 8 min: `None of the app's packages contain tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
