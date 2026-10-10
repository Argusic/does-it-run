# better-chatbot

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/keinsaasforever/better-chatbot, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/better-chatbot

## Pinned environment

- Project commit: `9c9ed86fd54d910ed22d0ad33576e1e6fbd1f43d`
- Test commit: `9c9ed86fd54d910ed22d0ad33576e1e6fbd1f43d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.3 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 11 | 11.3 | 4 | 4 | [run](https://argusic.com/run/80a5e144-6b62-41cc-8ecb-40fe01506158) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in PATH`
- 2 min: `Next.js 16 requires Node.js >=20.9.0, system has v18.19.1`
- 2 min: `Dev server instrumentation.ts calls process.exit(1) on DB migration failure, preventing launch without PostgreSQL`
- `No PostgreSQL in container (no root, no Docker)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
