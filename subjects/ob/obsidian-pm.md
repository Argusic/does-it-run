# obsidian-pm

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dotpm/obsidian-pm, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/obsidian-pm

## Pinned environment

- Project commit: `19d9f055ae3ce60a0753661b3fbe6ad39c98bd4d`
- Test commit: `19d9f055ae3ce60a0753661b3fbe6ad39c98bd4d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 3.8 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 16.1 | 4 | 4 | [run](https://argusic.com/run/0784c008-8b63-4e2f-b821-72fb10e46eb1) |
| 2 | pass with mocks | 92 | 4 | 3.8 | 1 | 1 | [run](https://argusic.com/run/52de2b5d-b4d5-4a68-a92d-20f6ec13111e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Environment Node 18 too old (project requires >=24)`
- 1 min: `pnpm not installed (project requires pnpm 11)`
- 1 min: `Transient 'Bad substitution' from dash sh on pnpm check:submission/check when the shell was busy`
- 3 min: `packages/api/dist is not standalone-runnable under plain Node because @dotpm/core exports point at src/index.ts with extensionless imports`

Attempt 2:

- 3 min: `Node.js v18 is too old (needs >=24); pnpm not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
