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
- Valid runs: 1; wall time 32.7 to 32.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 32.7 | 5 | 5 | [run](https://argusic.com/run/42f279eb-5429-449c-84a0-e409e4e147dc) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `PHP 8.4 not available in Ubuntu 24.04 apt repos (only 8.3)`
- 5 min: `Phar extension not compiled into PHP CLI binary`
- 2 min: `Composer.phar requires phar and iconv extensions`
- 2 min: `PHPUnit deb from Ubuntu has missing dependency chain`
- 5 min: `1 error (DumperNativeFallbackTest - needs SymfonyBridge ClassExistsMock), 16 failures (exit code 127 vs 252, no interactive terminal for QuestionHelper, StreamOutput newline handling)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
