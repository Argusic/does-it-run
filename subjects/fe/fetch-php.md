# fetch-php

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Thavarshan/fetch-php, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/fetch-php

## Pinned environment

- Project commit: `8c8342180e7f292c7bdef6948605d1aa723d0413`
- Test commit: `8c8342180e7f292c7bdef6948605d1aa723d0413`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.9 to 34.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 32 | 34.9 | 7 | 7 | [run](https://argusic.com/run/f239f546-bf62-40f3-90ee-b2f123226f65) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP 8.4 not installed in container`
- 5 min: `PeachPie PHP has phar/mbstring/iconv as loadable extensions, not built-in`
- 3 min: `Composer requires phar+mbstring+iconv extensions at startup`
- 5 min: `zip extension needs libzip.so.4 system library not available`
- 3 min: `phpstan/phpstan only distributes as zipball, blocking all dev deps install`
- 5 min: `Composer --prefer-source filled 5.9GB disk with VCS cache, ran out of space`
- 2 min: `PHPUnit needs dom/mbstring/tokenizer/xmlwriter extensions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
