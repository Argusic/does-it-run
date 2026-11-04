# crm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/trycompai/crm, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/crm

## Pinned environment

- Project commit: `6d4793dd6d7aeea91aa6a034e00b17d7408a2d08`
- Test commit: `6d4793dd6d7aeea91aa6a034e00b17d7408a2d08`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17.1 to 19.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 19.2 | 3 | 3 | [run](https://argusic.com/run/384a6b78-a780-4c6d-bf53-440cbf1f4e77) |
| 2 | pass | 100 | 19 | 17.1 | 3 | 3 | [run](https://argusic.com/run/587744d4-5d09-47c4-80f2-2cafacd73e57) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `bun install postinstall (prisma generate) fails with Node.js v18 because Prisma v7 uses ESM modules`
- 8 min: `Docker not available for PostgreSQL container`
- 1 min: `Postgres could not create /var/run/postgresql/.s.PGSQL.5432.lock (no root)`

Attempt 2:

- 8 min: `Prisma 7 CLI (ERR_REQUIRE_ESM) fails under system Node 18`
- 3 min: `Bun auto-loads .env with GOOGLE_CLIENT_ID="" causing test failure`
- 8 min: `Docker and Postgres unavailable in container , Postgres compiled from source`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
