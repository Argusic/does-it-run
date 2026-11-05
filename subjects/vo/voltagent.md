# voltagent

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/VoltAgent/voltagent, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/voltagent

## Pinned environment

- Project commit: `44b4c8e4998ce56095b2f0e4eaf1a988f5e6d0de`
- Test commit: `44b4c8e4998ce56095b2f0e4eaf1a988f5e6d0de`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 25.9 to 29.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 25.9 | 8 | 8 | [run](https://argusic.com/run/861b5159-08ac-40c5-b2b0-5d4139e26135) |
| 2 | pass with mocks | 92 | 1.6 | 29.6 | 7 | 7 | [run](https://argusic.com/run/931ba15e-a355-4186-8b76-5a3f1156259e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old (needs >=20) , pnpm install succeeded with warnings`
- 3 min: `8 packages failed vitest config load (vite 7 is ESM-only, config.cjs require() fails)`
- 2 min: `3 packages had no vitest config, test script failed with 'No projects found'`
- 1 min: `resumable-streams and voltagent-memory had no test files, vitest exited 1`
- 5 min: `server-elysia ElysiaServerProvider tests failed (port conflicts, mock mismatch with real impl)`
- 2 min: `evals vitest config was **/*.spec.ts which picked up duplicate tests from node_modules`
- 3 min: `scorers/autoeval.spec.ts and evals/run-experiment.spec.ts fail: transitive dep linear-sum-assignment requires() ESM-only ml-spectra-processing`
- 1 min: `@voltagent/e2e needs PostgreSQL (docker compose) on port 5433 , ECONNREFUSED`

Attempt 2:

- 4 min: `The system Node runtime was below the repository's Node >=20 requirement.`
- 1 min: `Example CLI bin links were missing after the initial frozen install.`
- 12 min: `Parallel pnpm test:all execution produced cross-package interference and port conflicts.`
- 3 min: `The E2E test command required Docker unconditionally, but Docker is unavailable in the container.`
- 4 min: `The Postgres E2E test failed when no database was reachable.`
- 10 min: `Elysia server tests asserted an obsolete mocked app.listen call and leaked listening servers between tests.`
- 6 min: `Three packages lacked local Vitest configuration, causing incorrect test discovery.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
