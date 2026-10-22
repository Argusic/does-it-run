# laravel-top

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leventcz/laravel-top, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/laravel-top

## Pinned environment

- Project commit: `1f2ba3c23ceddb0479444efc93d4be7e20fb04a2`
- Test commit: `1f2ba3c23ceddb0479444efc93d4be7e20fb04a2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 20.2 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 20.2 | 3 | 3 | [run](https://argusic.com/run/48d89b09-0f87-4185-b553-60d0da1db17a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP or Composer installed in the container (no root to apt install); required PHP 8.2+, ext-pcntl, and a Laravel app were absent`
- 8 min: `composer test script fails: phpstan analyse reports 13 errors (8 GuiBuilder nullsafe.neverNull, 1 Redis::pipeline() arguments.count, 4 unmatched ignore directives) and pint --test fails on 13 files (single_line_empty_body, new_with_parenthe`
- 31 min: `Could not stand up a real Redis server: no redis-server binary and system packages cannot be installed; an in-process stream-based fake Redis proved unreliable because the phpredis extension in the static build does not flush buffered reque`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
