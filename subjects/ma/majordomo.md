# majordomo

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sergejey/majordomo, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/majordomo

## Pinned environment

- Project commit: `d1283ab64ae94f82cce4226662d3b0662658c558`
- Test commit: `d1283ab64ae94f82cce4226662d3b0662658c558`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 15 to 42.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 13 | 15 | 5 | 5 | [run](https://argusic.com/run/ec48a65a-773c-4b12-b7af-5d8ae4a21f90) |
| 2 | pass | 100 | 41 | 42.5 | 6 | 6 | [run](https://argusic.com/run/03537d7f-bf03-41c2-85ee-d5592d319c72) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP interpreter in container`
- 5 min: `No MySQL/MariaDB in container`
- 2 min: `MariaDB crash recovery loop on restart`
- 1 min: `Stale unix socket from crashed mariadb`
- 1 min: `DB_HOST=localhost used default socket path not available`

Attempt 2:

- 5 min: `No PHP binary in container`
- 10 min: `No MySQL/MariaDB server available`
- 2 min: `MariaDB client requires libncurses.so.5, only libncursesw.so.6 is present`
- 2 min: `Missing cached_cycles table needed by caching.class.php`
- 3 min: `Invalid HTTP status headers in index.php and admin.php (#1 header malformed with colon and trailing newline)`
- 1 min: `DB_PORT not wired into mysqldb constructor`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
