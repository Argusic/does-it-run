# simslim

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MobAI-App/simslim, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/simslim

## Pinned environment

- Project commit: `f56a5a0e0ba04eb7315f7f1d624228ec68c80635`
- Test commit: `f56a5a0e0ba04eb7315f7f1d624228ec68c80635`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 4.8 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 7 | 4.8 | 1 | 1 | [run](https://argusic.com/run/ca1a9b6b-3d73-4124-8016-da2e65f24c57) |
| 2 | pass with mocks | 92 | 3.5 | 5.1 | 1 | 1 | [run](https://argusic.com/run/24fabbae-d4ce-4cd1-b637-2d9dabdc4c96) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `readPlistLabel called macOS-only plutil command, which doesn't exist on Linux, causing launchdJobPlists to return empty map and 7 tests to fail`

Attempt 2:

- 3.5 min: `readPlistLabel in launchd_batch.go called 'plutil' which is macOS-only; 8 tests failed on Linux because plutil was not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
