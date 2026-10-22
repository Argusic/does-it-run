# openreader

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/richardr1126/openreader, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openreader

## Pinned environment

- Project commit: `8af08e4622db96b36954d58b08b29e76c7ba723b`
- Test commit: `8af08e4622db96b36954d58b08b29e76c7ba723b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 7.6 to 18.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 18.1 | 0 | 0 | [run](https://argusic.com/run/37b54ff0-b4fa-47b9-9e3c-39568eb31d30) |
| 2 | pass with mocks | 92 | 20 | 7.6 | 6 | 6 | [run](https://argusic.com/run/7878fe97-e330-4669-9b96-0709ba37685d) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pnpm not found in PATH`
- 3 min: `Node.js v18 too old; vitest v4 requires node:util export styleText (Node 22+)`
- 1 min: `better-sqlite3 native module compiled for NODE_MODULE_VERSION 108 but Node v22 needs 127`
- 1 min: `14 tests failed: admin_providers and admin_settings tables missing`
- 1 min: `Production build failed: AUTH_SECRET not set`
- 1 min: `App startup failed: S3_INTERNAL_ENDPOINT required`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
