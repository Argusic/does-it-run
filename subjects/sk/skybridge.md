# skybridge

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alpic-ai/skybridge, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/skybridge

## Pinned environment

- Project commit: `8bc3175dcfd62f5aad970085b0be9f0faaba2e5e`
- Test commit: `8bc3175dcfd62f5aad970085b0be9f0faaba2e5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.1 to 44.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 39 | 44.1 | 3 | 3 | [run](https://argusic.com/run/d4928da1-8684-40a0-9c22-c0fab4051b6c) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Node.js v18.19.1 below required v24.18.0`
- 1 min: `pnpm not found in PATH`
- `Vite-plugin 2 tests timed out at 5000ms when run concurrently from root via pnpm -r, due to @babel/core cold-start latency`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
