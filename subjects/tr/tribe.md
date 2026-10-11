# tribe

**Verdict: runs.** Argusic Score 95.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/StreetLamb/tribe, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tribe

## Pinned environment

- Project commit: `e1c2020a7dd7377d1ec14292f113c53ddf50d917`
- Test commit: `e1c2020a7dd7377d1ec14292f113c53ddf50d917`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21 to 21 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95.56 | 25 | 21 | 9 | 7 | [run](https://argusic.com/run/9cf8abfd-203c-408f-81b9-08fde34c5d9b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `pystemmer build failed: Python.h not found (no python3-dev headers)`
- 4 min: `psycopg2 build failed: pg_config not found (no libpq dev headers)`
- 4 min: `No PostgreSQL available and no root to apt-install it`
- 3 min: `No Redis available for Celery broker/result backend`
- 2 min: `Backend settings fail without env vars (POSTGRES_*, PROJECT_NAME, CELERY_*, QDRANT_*, embedding models)`
- 1 min: `test_recovery_password failed: emails_enabled False`
- 1 min: `test_delete_upload returned 500 (Redis down)`
- 2 min: `test_create_upload FileNotFoundError '/app/upload-data/...' hardcoded Docker path; /app not creatable without root`
- 1 min: `app/tests/scripts/test_backend_pre_start.py and test_test_pre_start.py fail: 'called_once_with' is an invalid Mock assertion (upstream test bug, should be assert_called_once_with)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
