# opencode-manager

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chriswritescode-dev/opencode-manager, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opencode-manager

## Pinned environment

- Project commit: `c06075651dfeedce2b29462b260323655b4dfc87`
- Test commit: `c06075651dfeedce2b29462b260323655b4dfc87`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 33.1 to 33.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 33.1 | 6 | 6 | [run](https://argusic.com/run/984aefe1-4bfc-499b-8a85-c5d7592e25ca) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed`
- 3 min: `bun not installed`
- 8 min: `vitest: No such built-in module: node:sqlite`
- 5 min: `better-sqlite3 NODE_MODULE_VERSION mismatch (108 vs 109)`
- 1 min: `vitest: Failed to sync Assistant repository - transaction adapter mismatch`
- 1 min: `test/auth/index.test.ts: node:sqlite import in test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
