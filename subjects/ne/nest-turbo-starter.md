# nest-turbo-starter

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/typv/nest-turbo-starter, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/nest-turbo-starter

## Pinned environment

- Project commit: `93b761fee763dbed5e044af51d6a5d4f7847c775`
- Test commit: `93b761fee763dbed5e044af51d6a5d4f7847c775`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.3 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 8.3 | 4 | 4 | [run](https://argusic.com/run/a9249871-3209-4cd7-a651-2ffdff1b9115) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 below required >=20`
- 1 min: `pnpm not found - npm install -g failed (EACCES)`
- 1 min: `pnpm ignored build scripts for @swc/core, esbuild, @nestjs/core, protobufjs`
- 2 min: `Redis not available - app startup fails on ioredis connection`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
