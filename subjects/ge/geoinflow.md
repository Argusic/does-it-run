# GEOInflow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yaojingang/GEOInflow, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/geoinflow

## Pinned environment

- Project commit: `3d1504c480d66a7c0589b7e673a159ede6b268a9`
- Test commit: `3d1504c480d66a7c0589b7e673a159ede6b268a9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 40.3 to 40.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 40.3 | 8 | 8 | [run](https://argusic.com/run/04d26eee-e3b8-4ad9-9fbd-fb5b924408e6) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18.19.1 installed, project requires >=22 <23`
- 5 min: `PostgreSQL not available in container`
- 3 min: `Redis not available in container`
- 1 min: `initdb created lock dir /var/run/postgresql which doesn't exist`
- 1 min: `build:prisma:client required before liekan:migrate`
- 1 min: `OpenAPI generation failed because DATABASE_URL was in .env but tsx didn't load it`
- 1 min: `next dev watcher hit EMFILE (too many open files)`
- 2 min: `Production next build timed out after 180s in resource-constrained container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
