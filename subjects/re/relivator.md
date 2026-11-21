# relivator

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/reliverse/relivator, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/relivator

## Pinned environment

- Project commit: `a1871b006ab09df647b99fc71d3c080acd797e24`
- Test commit: `a1871b006ab09df647b99fc71d3c080acd797e24`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 7.6 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 8.5 | 2 | 2 | [run](https://argusic.com/run/13585b23-86ee-4584-b549-490b61c3a701) |
| 2 | pass with mocks | 92 | 9 | 7.6 | 4 | 4 | [run](https://argusic.com/run/e4016a7d-4e9a-456e-a6dc-79db52c649dd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun not found in PATH; npm install -g bun failed due to EACCES on /usr/local/lib/node_modules`
- 1 min: `next build failed with type error: 'User' type missing 'uploads' property in src/lib/queries/uploads.ts`

Attempt 2:

- 1 min: `bun runtime not available in container`
- 1 min: `bun test env.test.ts failed: DATABASE_URL had placeholder 'postgresql://...'`
- 1 min: `next build type error in src/lib/queries/uploads.ts: findMany return type conflicted with UserWithUploads which includes uploads relation`
- `next build OOM during static page generation (Generating static pages (0/18) killed by SIGKILL)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
