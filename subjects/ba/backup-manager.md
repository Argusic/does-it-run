# backup-manager

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/backup-manager/backup-manager, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/backup-manager

## Pinned environment

- Project commit: `fc986ad524babd90e382b511bdee3d8c3079941d`
- Test commit: `fc986ad524babd90e382b511bdee3d8c3079941d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.2 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.4 | 0 | 0 | [run](https://argusic.com/run/785093b3-07ba-4a02-af01-570fdaee8eca) |
| 2 | pass | 100 | 1.1 | 1.2 | 2 | 2 | [run](https://argusic.com/run/efc6625c-4542-41a7-b1e8-96cfc9704ae8) |

## What was observed on a clean machine

Attempt 2:

- 1.1 min: `PHP not installed in container (no root access for apt), installed static PHP 8.3.32 binary`
- 0.1 min: `ext-ftp missing from static PHP build, blocking composer install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
