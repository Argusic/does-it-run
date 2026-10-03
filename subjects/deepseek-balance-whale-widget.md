# DeepSeek-Balance-Whale-Widget

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MeteorNOX/DeepSeek-Balance-Whale-Widget, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/deepseek-balance-whale-widget

## Pinned environment

- Project commit: `770d3f55ff40284eb244fff33fc9ed4654be8a45`
- Test commit: `770d3f55ff40284eb244fff33fc9ed4654be8a45`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 23.7 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 29 | 30.3 | 2 | 2 | [run](https://argusic.com/run/d44d111c-82de-497a-9d83-08f3c4b9695e) |
| 2 | pass | 100 | 22 | 23.7 | 5 | 5 | [run](https://argusic.com/run/47ec1383-7ed9-469a-a49f-ebd76cdb9d47) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `dsh web server requires a PTY/TTY to stay alive and fails silently without one`

Attempt 2:

- 3 min: `Node.js v18 too old , DSH requires >=22; many packages required >=20`
- 2 min: `npm global install failed (EACCES , /usr/local locked down)`
- 5 min: `DSH profile not initialized; web profile had no package.json or bundle deps`
- 4 min: `Native binary node-addon-require-builtin-linux-x64-gnu not installed (optionalDependency npm skipped)`
- 3 min: `DSH web process exited silently after URL printed , nohup from wrong CWD lost module resolution`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
