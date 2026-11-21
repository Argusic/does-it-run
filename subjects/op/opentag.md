# opentag

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amplifthq/opentag, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opentag

## Pinned environment

- Project commit: `3a3136dcb8395b6dda6c872a8398d21a70935a23`
- Test commit: `3a3136dcb8395b6dda6c872a8398d21a70935a23`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.3 to 26.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 26.9 | 4 | 4 | [run](https://argusic.com/run/211aaf19-6687-41c6-83ad-b1b9c6773376) |
| 2 | pass | 100 | 4 | 5.3 | 1 | 1 | [run](https://argusic.com/run/139846f8-af06-43aa-810b-279da3fdb1cd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 is below the required >=22.14.0`
- 1 min: `corepack pnpm build failed: 'pnpm: not found' when the control-plane workspace spawned a nested pnpm`
- 3 min: `6 SQLite-backed tests exceeded the default 5000ms non-CI vitest timeout on this slow container`
- 6 min: `PostgreSQL 18 readiness incompatibility: PG18 catalogs NOT NULL constraints in pg_constraint, so control_plane_migrations has 4 constraints while the strict readiness query expects exactly 1 (migrations_pending)`

Attempt 2:

- 3 min: `Node.js v18.19.1 is too old; workspace packages require >=22.14.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
