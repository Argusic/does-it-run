# php-crud-api

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mevdschee/php-crud-api, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/php-crud-api

## Pinned environment

- Project commit: `399a398749ab687a68286260023bd73d79da5f26`
- Test commit: `399a398749ab687a68286260023bd73d79da5f26`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 5.2 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 6.4 | 0 | 0 | [run](https://argusic.com/run/dbddc0d7-e57b-4892-afe7-86761b473cff) |
| 2 | pass | 100 | 6.5 | 6.5 | 1 | 1 | [run](https://argusic.com/run/3fa0cae2-b006-41fe-82e6-a6163b1fe985) |
| 3 | pass | 100 | 5 | 5.2 | 2 | 2 | [run](https://argusic.com/run/d600dc94-3968-4e3b-8fa5-be200a149336) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `build.php failed to download phpfilemerger (SSL certificate verify failed)`

Attempt 3:

- 3 min: `PHP CLI not installed in container`
- 1 min: `pdo_sqlite extension_loaded() returns false for statically compiled PHP`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
