# churn-php

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bmitch/churn-php, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/churn-php

## Pinned environment

- Project commit: `d641760b9d21b37b7e1a30b80909d49ab7ff795f`
- Test commit: `d641760b9d21b37b7e1a30b80909d49ab7ff795f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 41.4 to 41.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 41 | 41.4 | 7 | 7 | [run](https://argusic.com/run/e93c7ff2-3d51-4e18-ab50-af7cbb962a11) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `PHP 8.3 interpreter not installed`
- 5 min: `Composer installer phar had broken signature`
- 3 min: `Simple-phpunit test runner could not find composer binary`
- 6 min: `PHP zip extension required libzip.so.4 which was missing`
- 2 min: `PHP DOM extension required for phar-io/manifest`
- 2 min: `PHP mbstring extension required for phpunit install`
- `5 pre-existing test failures in FileHelperTest for Windows path handling on Linux`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
