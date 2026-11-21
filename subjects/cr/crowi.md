# crowi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crowi/crowi, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/crowi

## Pinned environment

- Project commit: `c96e47fe76ab36a93662a80a76c121d13a93657e`
- Test commit: `c96e47fe76ab36a93662a80a76c121d13a93657e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 18.7 to 50.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 50.3 | 2 | 2 | [run](https://argusic.com/run/cef92007-ab87-43e1-b9b4-b4a2f63446bc) |
| 2 | pass | 100 | 18 | 18.7 | 8 | 8 | [run](https://argusic.com/run/d75bc19b-2a1a-4b7b-b79d-097233385817) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `@crowi/api-contract DTS build OOM'd with default heap (container has 772MB, DTS rollup needs ~3GB+ for 2.5MB .d.ts)`
- 1 min: `MongoDB binary lockfile conflict between postinstall (8.2.6) and test (8.0.4) versions`

Attempt 2:

- 2 min: `System Node.js v18.19.1 does not satisfy engines.node (24.x)`
- 1 min: `pnpm not found (corepack not available on system Node 18)`
- 3 min: `pnpm install blocked build scripts for @parcel/watcher, esbuild, lefthook, mongodb-memory-server, unrs-resolver`
- 1 min: `api-contract DTS build OOM (ERR_WORKER_OUT_OF_MEMORY)`
- 1 min: `API tsc build OOM on tsc`
- 2 min: `API tsc build failed: 40+ TS2307 errors for @crowi/plugin-api, @crowi/collab, @crowi/runner, @crowi/plugin-storage-local etc.`
- 1 min: `plugin-storage-aws-s3 DTS build failed requiring @crowi/plugin-aws dts`
- 4 min: `mongodb-memory-server per-file startup timeout for 17 test suites (10s timeout exceeded under memory pressure)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
