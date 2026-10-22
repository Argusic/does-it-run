# reactpress

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fecommunity/reactpress, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/reactpress

## Pinned environment

- Project commit: `b482b97072ba976df518fa485748739815142473`
- Test commit: `b482b97072ba976df518fa485748739815142473`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 57.9 to 57.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 57.9 | 7 | 7 | [run](https://argusic.com/run/919e0d51-c0a5-4dc6-af4b-aa9d63e150c1) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm postinstall failure - cli/toolkit symlink missing`
- 2 min: `cli/server/node_modules wiped by pnpm prepare`
- 0.5 min: `Toolkit dist empty after install`
- 0.5 min: `cli/server/dist/main.js doesn't export main()`
- 0.5 min: `Missing nginx templates in cli/templates/`
- 0.5 min: `react/jsx-runtime and next not found at runtime by toolkit dist`
- `Admin SPA (web) build fails on Node 18 - vite-plus requires styleText from node:util (Node >=21.7)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
