# dbal

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/doctrine/dbal, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/dbal

## Pinned environment

- Project commit: `205fdf552ffafe33c1d12a41a2d6c7217666c32c`
- Test commit: `205fdf552ffafe33c1d12a41a2d6c7217666c32c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.4 to 10.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.3 | 10.4 | 2 | 2 | [run](https://argusic.com/run/c5f9210e-3380-4314-8457-e91ba404d178) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `extension_loaded('pdo_sqlite') returns false for static PHP builds even when the PDO SQLite driver is present and usable via PDO::getAvailableDrivers()`
- 1.5 min: `PHP 8.3.28 static build does not include the getColumnMeta-fix-on-freed-statement from php-src#17837 despite being above the version threshold (8.3.18), causing testColumnNameAfterFree to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
