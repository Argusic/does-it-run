# filament-kanban

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mokhosh/filament-kanban, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/filament-kanban

## Pinned environment

- Project commit: `76bd44d71dc01fd02d4fd635d55b17af1f497eaf`
- Test commit: `76bd44d71dc01fd02d4fd635d55b17af1f497eaf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 5.4 | 2 | 2 | [run](https://argusic.com/run/cfcdc36b-91ef-4024-ad6d-2ba881e5433d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container had no PHP and no root to apt install it (Ubuntu 24.04, runner user)`
- 1 min: `composer install was blocked by Composer 2.11's new security-advisory policy rejecting older Laravel 10/11 releases required by orchestra/testbench (repo has no composer.lock)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
