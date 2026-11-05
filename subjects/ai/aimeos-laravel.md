# aimeos-laravel

**Verdict: runs with mocks.** Argusic Score 90.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aimeos/aimeos-laravel, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/aimeos-laravel

## Pinned environment

- Project commit: `9879c60332e9fc6611450be9879f5eb1a93c887c`
- Test commit: `9879c60332e9fc6611450be9879f5eb1a93c887c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 27 to 41.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 89.14 | 32 | 27 | 7 | 6 | [run](https://argusic.com/run/7b1282bb-5ebb-4cad-ad43-5bca7cc51564) |
| 2 | pass with mocks | 92 | 8 | 41.2 | 2 | 2 | [run](https://argusic.com/run/dc9c263a-0979-42f1-8fd3-25fc751df67b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No PHP runtime pre-installed in container`
- 2 min: `No Composer pre-installed`
- 5 min: `No MySQL server available (no root, no Docker)`
- 3 min: `intl extension (NumberFormatter) not in the common PHP build`
- 5 min: `SQLite doesn't support ANSI OFFSET...FETCH NEXT syntax`
- 2 min: `vendor/aimeos/aimeos-core/Setup.php missing sqlite driver mapping`
- `7 out of 8 Base tests pass; 2 need database tables with seed data; all command/controller tests need a populated MySQL database`

Attempt 2:

- 45 min: `MySQL server not available in container (no root, no portable binary), database tests cannot execute`
- 5 min: `PHP ext-intl extension missing in static PHP 8.4 build, required by aimeos/aimeos-core`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
