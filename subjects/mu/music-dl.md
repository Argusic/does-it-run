# music-dl

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/guanguans/music-dl, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/music-dl

## Pinned environment

- Project commit: `b3958044a3ca76ec012ff4938cc93bee2c3a918b`
- Test commit: `b3958044a3ca76ec012ff4938cc93bee2c3a918b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 26.7 to 36.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 6 | 36.3 | 3 | 3 | [run](https://argusic.com/run/aa6f6687-2f8c-4257-8b43-826eaa6e9c33) |
| 2 | pass | 100 | 62 | 26.7 | 5 | 5 | [run](https://argusic.com/run/42e5344e-16e2-402e-a08a-36a784b1ddaf) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `PHP and Composer are not installed and no root is available to install system packages.`
- 1 min: `The static PHP build lacks the pdo_sqlite driver (only pdo_mysql available), needed by the SQLite test setup.`
- 1 min: `composer install was not completed, so vendor/ was not created and the test suite could not run.`

Attempt 2:

- 8 min: `No PHP runtime or Composer present in container (Ubuntu 24.04, no root); README requires PHP >= 8.5`
- 10 min: `composer install failed: locked php-standard-library/date-time, locale, process require ext-intl which was missing from the default static PHP build`
- 35 min: `composer test (pest) fails with 'No code coverage driver is available' because static PHP has no xdebug/pcov and spc declares pcov shared-only, so --coverage cannot run; tests themselves pass`
- 3 min: `A brand-new user running './music-dl --version'/'list' gets '/usr/bin/env: php': No such file or directory' unless php is on PATH`
- 6 min: `CLI music search with fresh, non-existent --directory fails validation; kugou and tencent download-URL endpoints return empty URLs from this container (region/licensing), so searches list zero songs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
