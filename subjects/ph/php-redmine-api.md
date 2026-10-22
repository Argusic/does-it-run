# php-redmine-api

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kbsali/php-redmine-api, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/php-redmine-api

## Pinned environment

- Project commit: `ab0c715114e43f24d5bdb2aa532dccc828f55679`
- Test commit: `ab0c715114e43f24d5bdb2aa532dccc828f55679`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.3 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10.7 | 0 | 0 | [run](https://argusic.com/run/a4c36fcd-fad9-406a-8e57-ed37143f483c) |
| 2 | pass | 100 | 10 | 6.3 | 3 | 3 | [run](https://argusic.com/run/6123452f-8ff4-4a16-8355-b1edbb661e55) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `PHP not installed in container; required ext-curl, ext-simplexml, ext-json`
- 1 min: `Composer not installed`
- 5 min: `4 PHPUnit test failures: libxml 2.15.3 produces different error messages than tests expected (empty string error code 3 vs 0, no 'Extra content' messages)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
