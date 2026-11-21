# esengine

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/esengine/esengine, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/esengine

## Pinned environment

- Project commit: `2886284e8015c57ad8a0ef89596a058890cfa679`
- Test commit: `2886284e8015c57ad8a0ef89596a058890cfa679`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 6.2 | 7 | 3 | 1 | [run](https://argusic.com/run/5cd65e9f-91ea-4418-8141-30192dca6a9d) |
| 2 | pass | 100 | 9 | 9.5 | 3 | 3 | [run](https://argusic.com/run/b59bb6bb-7ec6-4006-9437-39759eed0472) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `@esengine/docs requires Node.js >=18.20.8, container has 18.19.1`
- 1.5 min: `@esengine/transaction::SagaOrchestrator test: saga state set to 'failed' instead of 'compensated' after successful compensation`
- `@esengine/pathfinding::ORCABenchmark test: perf benchmark timed out (22ms vs 16.67ms budget)`

Attempt 2:

- 1 min: `pnpm not installed in container`
- `Docs package fails to build - Astro requires Node.js >= 18.20.8, container has 18.19.1`
- 5 min: `Transaction SagaOrchestrator test fails: compensation detection logic incorrectly marks execution-failed steps as compensation failures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
