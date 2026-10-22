# badaso

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/uasoft-indonesia/badaso, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/badaso

## Pinned environment

- Project commit: `b47266534aea33611d480d88f0f5819e07a708cb`
- Test commit: `b47266534aea33611d480d88f0f5819e07a708cb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.7 to 22.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 22.7 | 5 | 5 | [run](https://argusic.com/run/13f15925-c0ae-4a27-bc47-c6caeff75809) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP not installed in container`
- 1 min: `Composer not installed`
- `Composer security advisories blocking package installs for league/flysystem, laravel/framework, firebase/php-jwt, unisharp/laravel-filemanager`
- 3 min: `Migration 2022_03_08_090850 fails with Call to undefined method Doctrine\DBAL\Connection::createSchemaManager() because doctrine/dbal 2.13.9 is pinned but Laravel 10 requires DBAL 3.x schema API`
- `BadasoApiCrudManagementTest hangs/times out creating tables with SQLite on static PHP build and Schema::hasTable() triggers Doctrine DBAL`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
