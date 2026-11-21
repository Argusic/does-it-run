# project-management

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/devaslanphp/project-management, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/run/69aab2e1-4a42-46ed-83f0-3fd1f74ee425

## Pinned environment

- Project commit: `54982160896d8371ba79c8dc20ed65936878d91b`
- Test commit: `54982160896d8371ba79c8dc20ed65936878d91b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 6.5 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 12.4 | 5 | 5 | [run](https://argusic.com/run/69aab2e1-4a42-46ed-83f0-3fd1f74ee425) |
| 2 | pass with mocks | 92 | 14 | 6.5 | 5 | 5 | [run](https://argusic.com/run/4cf669f0-e078-4e45-a50a-6b8e48ab5def) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP runtime available on the system`
- 3 min: `PHP 8.5 (latest FrankenPHP) too new for composer.lock and dependency constraints (<8.3)`
- 3 min: `Composer phar argv[0] mismatch with FrankenPHP php-cli mode`
- 1 min: `Settings migration table missing UNIQUE(group,name) constraint, causing seeder to fail with SQLite upsert error`
- 1 min: `Feature test expected HTTP 200 on / but app redirects unauthenticated users (302)`

Attempt 2:

- 3 min: `No PHP runtime in container`
- 1 min: `No Composer in container`
- 1 min: `composer.lock packages require PHP <8.3, default PHP 8.3 too new`
- 1 min: `No MySQL database available`
- 1 min: `Deprecated explode(null) in config/services.php`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
