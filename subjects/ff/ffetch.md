# ffetch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fetch-kit/ffetch, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ffetch

## Pinned environment

- Project commit: `f20c1c383e67da49dbefc6bc3f208be541cf8fdf`
- Test commit: `f20c1c383e67da49dbefc6bc3f208be541cf8fdf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.4 | 4 | 4 | [run](https://argusic.com/run/42221cf9-f4e9-44b8-b860-cef6dd256b47) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node 18 lacks node:util.styleText (v20.12+ API) required by vitest/rolldown; npm test crashed at startup`
- 2 min: `Fresh npm install with npm 10 crashed: Cannot read properties of null (reading 'edgesOut')`
- 1 min: `Rolldown native binding missing after initial install (Cannot find native binding, asked for wasm fallback)`
- 1 min: `Smoke script imported nonexistent dist/plugins/retry.js (retry is built-in, not a plugin)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
