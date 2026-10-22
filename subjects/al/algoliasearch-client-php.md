# algoliasearch-client-php

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/algolia/algoliasearch-client-php, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/algoliasearch-client-php

## Pinned environment

- Project commit: `385047851b8ba74ec42e89c918b7517ee312d8cc`
- Test commit: `385047851b8ba74ec42e89c918b7517ee312d8cc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.8 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 8.8 | 4 | 4 | [run](https://argusic.com/run/1874fd62-a843-4a0b-b93c-17cf18ca98d7) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `No PHP or Composer installed in container and no root to apt-get install`
- 3 min: `Composer install failed: zip extension and unzip/7z both missing`
- `composer test not defined (no scripts in composer.json); phpunit.xml.dist points at missing generated CTS dir ../../tests/output/php/src/ so vendor/bin/phpunit cannot run any tests`
- 2 min: `phpstan level max reported 13033 findings (mostly type-doc on generated code); first run crashed on 128M memory limit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
