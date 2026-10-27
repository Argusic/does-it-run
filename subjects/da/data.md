# data

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/atk4/data, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/data

## Pinned environment

- Project commit: `2cbd3dbc2dd3cb7655055dcdd34b4c4eb2c873f9`
- Test commit: `2cbd3dbc2dd3cb7655055dcdd34b4c4eb2c873f9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.3 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 7.3 | 1 | 1 | [run](https://argusic.com/run/f6310062-0d36-4893-b944-8d897b26b7b7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Test testConnectInvalidHostException failed: static PHP binary lacked 'mysqli' extension, causing fatal error 'Class mysqli not found' when connecting with DSN scheme 'mysql:' (which maps to mysqli driver)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
