# intentkit

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crestalnetwork/intentkit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/intentkit

## Pinned environment

- Project commit: `afc8cc44255210db6352f7437e569ed8b88ed5e1`
- Test commit: `afc8cc44255210db6352f7437e569ed8b88ed5e1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 27.6 to 55.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 36 | 55.8 | 2 | 2 | [run](https://argusic.com/run/cf5e0bec-cd3b-4cbf-a2fc-ad8a456d5077) |
| 2 | pass | 100 | 35 | 27.6 | 6 | 6 | [run](https://argusic.com/run/137faac0-f33f-42db-8d2e-af1a5ebc54bc) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `psycopg required libpq which was not found; added psycopg-binary wheel`
- 30 min: `PostgreSQL server binaries (initdb+postgres) not pre-installed and extracted debs postmaster is blocked by Docker AppArmor profile 'docker-default (enforce)'`

Attempt 2:

- 2 min: `uv not installed in container`
- 1 min: `Python 3.13 not available`
- 8 min: `psycopg import fails: no pq wrapper (libpq not found)`
- 3 min: `testing.postgresql cannot find initdb/postgres`
- 3 min: `BDD tests fail without Redis running`
- 1 min: `API server startup fails without .env`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
