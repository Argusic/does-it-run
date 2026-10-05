# typeorm

**Verdict: runs.** Argusic Score 71.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/typeorm/typeorm, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/8400c6f7-5400-4308-8104-396161f0e19c

## Pinned environment

- Project commit: `ac41823b9e27e3a8079ce487c9772c5ef8f1e226`
- Test commit: `ac41823b9e27e3a8079ce487c9772c5ef8f1e226`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 12.4 to 53.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.4 | 2 | 2 | [run](https://argusic.com/run/8400c6f7-5400-4308-8104-396161f0e19c) |
| 2 | fail | 20 | n/a | 40.5 | 0 | 0 | [run](https://argusic.com/run/264e8666-062e-4154-902a-e377d1dd4b8b) |
| 3 | pass | 93.33 | 13 | 53.3 | 6 | 4 | [run](https://argusic.com/run/88a3853b-c2a9-4b70-9015-88fc7f457fe6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18.19.1 below required engine (^20.19.0 || ^22.13.0)`
- 1 min: `pnpm not found on PATH`

Attempt 3:

- 1 min: `pnpm version mismatch - project requires ^10.34.5`
- 3 min: `chai v6 is ESM-only, Node 18 cannot require('chai/register-should')`
- 2 min: `File is not defined - undici (testcontainers dependency) requires Node 20+ File global`
- 7 min: `better-sqlite3 native addon compiled against NODE_MODULE_VERSION 108 but Debian Node 18.19.1 expects 109`
- `yargs v18 is ESM-only, CLI init test cannot require() it on Node 18`
- `Redis testcontainers test requires Docker runtime, none available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
