# pezzo

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pezzolabs/pezzo, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pezzo

## Pinned environment

- Project commit: `0787e3c037ad24544c2d3e6842507c3e7461a1de`
- Test commit: `0787e3c037ad24544c2d3e6842507c3e7461a1de`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.7 to 19.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 19.7 | 2 | 2 | [run](https://argusic.com/run/d12c3437-f075-4d73-a83e-a28b9a3abaef) |

## What was observed on a clean machine

Attempt 1:

- `No Docker in container, so PostgreSQL/ClickHouse/Redis/Supertokens infra not available for true end-to-end startup`
- `Prisma cannot connect to PostgreSQL on port 5432 (no Postgres running)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
