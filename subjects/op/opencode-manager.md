# opencode-manager

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chriswritescode-dev/opencode-manager, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opencode-manager

## Pinned environment

- Project commit: `c06075651dfeedce2b29462b260323655b4dfc87`
- Test commit: `c06075651dfeedce2b29462b260323655b4dfc87`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 21.7 to 33.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 33.1 | 6 | 6 | [run](https://argusic.com/run/984aefe1-4bfc-499b-8a85-c5d7592e25ca) |
| 2 | pass | 100 | 21 | 21.7 | 4 | 4 | [run](https://argusic.com/run/926763cc-36c0-4a14-87a4-be41d3e3ce28) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed`
- 3 min: `bun not installed`
- 8 min: `vitest: No such built-in module: node:sqlite`
- 5 min: `better-sqlite3 NODE_MODULE_VERSION mismatch (108 vs 109)`
- 1 min: `vitest: Failed to sync Assistant repository - transaction adapter mismatch`
- 1 min: `test/auth/index.test.ts: node:sqlite import in test`

Attempt 2:

- 3 min: `Bun runtime not installed on system`
- 2 min: `pnpm package manager not installed`
- 2 min: `Node.js v18.19.1 too old for Vite 7 (needs 20.19+/22.12+)`
- 3 min: `unzip binary not found, causing 8 test failures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
