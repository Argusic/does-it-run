# dramaxis

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Agions/dramaxis, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dramaxis

## Pinned environment

- Project commit: `03347b261d0545b987aa6c63f48e1d4c3c7294bd`
- Test commit: `03347b261d0545b987aa6c63f48e1d4c3c7294bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.2 to 11.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.2 | 6 | 6 | [run](https://argusic.com/run/d8112b99-107f-4e38-88b9-5aa32cd4e49f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm package manager not found`
- 2 min: `Node.js 18 too old for Vite 7 (requires Node 20.19+/22.12+)`
- 1 min: `vite.config.ts uses import.meta.dirname (Node 20.11+ API) which fails on Node 18`
- 1 min: `pnpm rejected esbuild builds (approve-builds needed)`
- 1 min: `@tailwindcss/oxide-linux-x64-gnu native binding missing after Node upgrade`
- 5 min: `Tauri system library libwebkit2gtk-4.1-dev missing (no root access)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
