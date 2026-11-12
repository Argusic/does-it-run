# mcp-server-mysql

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/benborla/mcp-server-mysql, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/mcp-server-mysql

## Pinned environment

- Project commit: `b9c714e182422b9f18437242b80cf003adf1c7ea`
- Test commit: `b9c714e182422b9f18437242b80cf003adf1c7ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 15.6 to 17.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 17.1 | 3 | 3 | [run](https://argusic.com/run/02c739c6-31ba-4924-a3ee-217ffd72c444) |
| 2 | pass | 100 | 15 | 15.6 | 6 | 6 | [run](https://argusic.com/run/ef3a7cf9-61f5-4454-b889-eb527535df1d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `dotenv.config() loaded .env before vitest stubs, breaking env-override in 3 unit tests`
- 5 min: `Fatal safeExit(1) on DB connection test failure killed remote HTTP server at startup`
- 3 min: `executeReadOnlyQuery test didn't expect new timing entry in response`

Attempt 2:

- 1 min: `Node.js v18.19.1 does not meet minimum v20 requirement`
- 3 min: `MySQL server not installed and no root/sudo to install packages`
- 2 min: `MySQL server process was killed when parent shell exited (process group signal)`
- 1 min: `pnpm 12 required but not available`
- 1 min: `Vitest config files (vitest.unit.config.ts, vitest.integration.config.ts, vitest.e2e.config.ts) referenced in package.json are missing from the repository`
- 5 min: `Test failures: 10 tests failed - schema permissions tests expected write operations to be blocked but .env.test had all allow flags set to true, and multi-DB USE statement test failed due to missing multipleStatements config`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
