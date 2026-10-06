# coolify

**Verdict: runs.** Argusic Score 91.4 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coollabsio/coolify, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/coolify

## Pinned environment

- Project commit: `34e4da1095726c6f9e4bb4272aa01b5a6dd43901`
- Test commit: `34e4da1095726c6f9e4bb4272aa01b5a6dd43901`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.9 to 21.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 91.43 | 22 | 21.9 | 7 | 4 | [run](https://argusic.com/run/1d0e4757-1c2f-4a32-b2f8-c1ad8d0f5dee) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `PHP 8.3 used instead of PHP ^8.4 (composer require) - PHP 8.4 not available in Ubuntu repos`
- 8 min: `Composer installer requires phar, iconv, mbstring extensions - PHP CLI binary built without these`
- 2 min: `Composer needs zip extension but zip.so requires libzip.so.4 - not available in container`
- 2 min: `Laravel artisan needs PDO SQLite driver for testing DB connection`
- `704 unit tests fail - pre-existing, need running Postgres/Docker servers`
- `Browser tests skipped - Playwright not installed`
- `Feature tests timeout - may need more memory or contain interactive tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
