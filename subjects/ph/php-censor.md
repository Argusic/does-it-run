# php-censor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/php-censor/php-censor, licensed BSD-2-Clause, written in PHP.

Evidence and recordings: https://argusic.com/subject/php-censor

## Pinned environment

- Project commit: `7b8e6404b7126caf972a2b993a635250b54dc0da`
- Test commit: `7b8e6404b7126caf972a2b993a635250b54dc0da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 12.4 | 5 | 5 | [run](https://argusic.com/run/c060978c-7697-4ece-80ff-32164118baa6) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `PHP not installed in container`
- 0.2 min: `Composer not installed in container`
- 0.1 min: `php not on PATH (env: 'php' not found by tests)`
- 0.2 min: `PHP 8.3 deprecation: ${var} string interpolation in InstallCommand.php:232`
- 0.1 min: `PHP 8.3 deprecation: ${var} string interpolation in SvnBuild.php:59`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
