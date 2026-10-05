# mcp-server-mysql

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/benborla/mcp-server-mysql, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/mcp-server-mysql

## Pinned environment

- Project commit: `b9c714e182422b9f18437242b80cf003adf1c7ea`
- Test commit: `b9c714e182422b9f18437242b80cf003adf1c7ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.1 to 17.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 17.1 | 3 | 3 | [run](https://argusic.com/run/02c739c6-31ba-4924-a3ee-217ffd72c444) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `dotenv.config() loaded .env before vitest stubs, breaking env-override in 3 unit tests`
- 5 min: `Fatal safeExit(1) on DB connection test failure killed remote HTTP server at startup`
- 3 min: `executeReadOnlyQuery test didn't expect new timing entry in response`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
