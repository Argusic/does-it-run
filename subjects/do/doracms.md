# DoraCMS

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/doramart/DoraCMS, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/doracms

## Pinned environment

- Project commit: `bdaded858ce655fccae0c01c18e36e420c5c48fe`
- Test commit: `bdaded858ce655fccae0c01c18e36e420c5c48fe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 25.8 to 50.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 50.1 | 7 | 7 | [run](https://argusic.com/run/fa6f89f1-b0b4-408c-a596-866939b3278d) |
| 2 | pass with mocks | 92 | 1.5 | 25.8 | 4 | 4 | [run](https://argusic.com/run/c72f7174-a9ea-47cc-ae86-d6cf1a1409de) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in container`
- 2 min: `pnpm install blocked build scripts for 10 packages`
- 5 min: `globalThis.File not defined in Node 18 causing undici@7 to crash`
- 4 min: `EventSource is not a constructor in egg-watcher on Node 18`
- 3 min: `env.js getEnv returns default even when env var is explicitly empty string (REDIS_HOST=)`
- 5 min: `MongoDB not available for integration tests`
- `Integration tests still fail due to Node 18 compatibility (Cannot delete property 'service'), mock context issues, and missing Redis`

Attempt 2:

- 5 min: `Egg-watcher package missing "none" event source - tests using config.watcher = {type: "none"} crashed with EventSource is not a constructor`
- 1 min: `Missing test/mock_data.js - content-publish-ai.test.js could not load`
- 2 min: `Missing test fixtures for framework test (service + favicon)`
- `Server cannot start without Redis - Bull queue crashes on startup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
