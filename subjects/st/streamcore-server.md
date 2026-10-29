# streamcore-server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/streamcoreai/streamcore-server, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/streamcore-server

## Pinned environment

- Project commit: `71878ec29ad017f688565ae123f84f1d9da662ab`
- Test commit: `71878ec29ad017f688565ae123f84f1d9da662ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 4.9 | 2 | 2 | [run](https://argusic.com/run/2f30fd3b-6190-4576-a248-37e4b037bfdc) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.25 was not installed in the container`
- `4 plugins (gmail, math-calculate, time-get, weather-get) failed to load due to missing SDK packages (@streamcore/plugin, streamcoreai_plugin, and EACCES on /work/plugin-sdk)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
