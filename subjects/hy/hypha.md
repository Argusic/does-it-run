# Hypha

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CodeSoul-co/Hypha, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hypha

## Pinned environment

- Project commit: `ac77fa9b4a1b1da2815adf7d5582dbc27cd9373f`
- Test commit: `ac77fa9b4a1b1da2815adf7d5582dbc27cd9373f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 36.5 to 36.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 36.5 | 4 | 4 | [run](https://argusic.com/run/4877b3a1-20d0-4669-8d4b-ca8b11167855) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container shipped Node 18.19.1 but repo requires Node >=22 (engine + .nvmrc 22.22.3); no nvm/fnm and no root for system packages`
- 8 min: `MongoDB and Redis were absent and Docker (for bundled compose) unavailable; integration tests and the API server require them`
- 5 min: `memory-native production-topology acceptance failed 1/6: after a force primary stepdown the same RS node regained primary, so the test never saw a different primary within 45s`
- 1 min: `2 MCP performance tests flaked under full parallel npm test (refresh_10000_ms 8288ms > 5000ms threshold) but passed in isolation and in the full packages run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
