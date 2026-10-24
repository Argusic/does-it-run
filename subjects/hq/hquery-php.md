# hQuery.php

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/duzun/hQuery.php, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/hquery-php

## Pinned environment

- Project commit: `50a9f211b47e778bd40660906466391104efed3b`
- Test commit: `50a9f211b47e778bd40660906466391104efed3b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.3 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 7.3 | 3 | 3 | [run](https://argusic.com/run/92276ea7-a6cc-40b4-beae-4b52ac42df4e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP binary installed in container`
- 1 min: `SSL cert failure downloading composer installer via copy()`
- 2 min: `phpunit not in composer require-dev`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
