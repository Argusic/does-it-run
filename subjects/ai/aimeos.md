# aimeos

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aimeos/aimeos, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/aimeos

## Pinned environment

- Project commit: `919720089ad5ff6e63eee9c0aaf4a42c2cc27340`
- Test commit: `919720089ad5ff6e63eee9c0aaf4a42c2cc27340`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 22.4 to 68 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 38 | 68 | 9 | 9 | [run](https://argusic.com/run/8e93e50a-7bc9-4131-9dfd-3f43f0c07f2e) |
| 2 | pass with mocks | 92 | 16 | 22.4 | 7 | 7 | [run](https://argusic.com/run/b04a684e-4c5d-481e-824b-a12d9087aa3b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP not installed in container`
- 1 min: `Composer not installed`
- 1 min: `ext-intl missing from default static PHP build`
- 1 min: `No .env file (project was cloned, not create-project)`
- 2 min: `MySQL not available in container`
- 5 min: `SQL OFFSET...ROWS FETCH NEXT...ROWS ONLY syntax unsupported by SQLite`
- 3 min: `LAST_INSERT_ID() is MySQL function, unsupported by SQLite`
- 1 min: `DO GET_LOCK/RELEASE_LOCK is MySQL-specific, unsupported by SQLite`
- 3 min: `Aimeos DB tables not created in testing database`

Attempt 2:

- 2 min: `PHP and Composer not available in container`
- 3 min: `Aimeos vendor SQL uses SQL Server syntax (OFFSET ... ROWS FETCH NEXT ... ROWS ONLY) incompatible with SQLite`
- 1 min: `Laravel config/database.php used 'sqlite' driver but Upscheme connect macro in vendor/aimeos/aimeos-core/Setup.php didn't map 'sqlite' to 'pdo_sqlite'`
- 3 min: `Doctrine PDO SQLite driver expects 'path' parameter not 'dbname'`
- 1 min: `Shop resource config passed relative 'laravel.sqlite' path which Doctrine/SQLite couldn't resolve`
- 1 min: `The 'newid' SQL config (for getting last insert ID) lacked SQLite entry`
- 2 min: `PHP built-in server hangs on real requests (timeout on curl)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
