# OpenAgentCore

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MiniMax-AI/OpenAgentCore, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/openagentcore

## Pinned environment

- Project commit: `daeb75465fac518ccd336f5e34b251eb136dcefe`
- Test commit: `daeb75465fac518ccd336f5e34b251eb136dcefe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 48.6 to 48.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 48 | 48.6 | 4 | 4 | [run](https://argusic.com/run/52cd7450-87bd-4ea1-b3d5-6627e1f4ac5c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in container`
- 5 min: `PostgreSQL not installed , all Core database tests would be skipped`
- 1 min: `pnpm not installed , needed for web/frontend builds and tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
