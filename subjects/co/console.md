# console

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/symfony/console, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/console

## Pinned environment

- Project commit: `440fb189f48a65d91cb62e2de7da18b41f6db541`
- Test commit: `440fb189f48a65d91cb62e2de7da18b41f6db541`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.8 to 32.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 32.7 | 5 | 5 | [run](https://argusic.com/run/42f279eb-5429-449c-84a0-e409e4e147dc) |
| 2 | pass | 100 | 12 | 14.8 | 6 | 6 | [run](https://argusic.com/run/492afb8b-a838-43de-962a-60558da0f9d5) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `PHP 8.4 not available in Ubuntu 24.04 apt repos (only 8.3)`
- 5 min: `Phar extension not compiled into PHP CLI binary`
- 2 min: `Composer.phar requires phar and iconv extensions`
- 2 min: `PHPUnit deb from Ubuntu has missing dependency chain`
- 5 min: `1 error (DumperNativeFallbackTest - needs SymfonyBridge ClassExistsMock), 16 failures (exit code 127 vs 252, no interactive terminal for QuestionHelper, StreamOutput newline handling)`

Attempt 2:

- 4 min: `No PHP interpreter in the container`
- 2 min: `No Composer in the container`
- 1 min: `phpunit not in dev dependencies`
- 1 min: `symfony/phpunit-bridge missing from dev dependencies`
- 1 min: `phpunit.xml.dist had invalid attribute ignoreUndefinedTriggers on deprecationTrigger element and referenced Doctrine Deprecations methods not in dependencies`
- `3 pre-existing test failures due to version mismatch between test expectations and installed symfony/lock 8.2.x-dev and environment constraints`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
