# digarr

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iuliandita/digarr, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/digarr

## Pinned environment

- Project commit: `b65a8f5dca34d5a9a16339b82e4184581449d897`
- Test commit: `b65a8f5dca34d5a9a16339b82e4184581449d897`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 7.8 | 3 | 3 | [run](https://argusic.com/run/3df5973b-de4a-43a8-96dc-417b10a5dc59) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Bun not installed , Node 18.19.1 was the only runtime`
- 1 min: `Node 18.19.1 lacks node:util.styleText , vitest 5/Vite 8 rolldown crashes with SyntaxError`
- `15 test failures in 5 files: session-queries (5), oidc-link-postgres (4), oidc-token-retirement (1), sync-flow (4), reconciler-cache (1) , all ECONNREFUSED 127.0.0.1:5432`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
