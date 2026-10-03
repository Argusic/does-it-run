# aimeos-laravel

**Verdict: runs with mocks.** Argusic Score 89.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aimeos/aimeos-laravel, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/aimeos-laravel

## Pinned environment

- Project commit: `9879c60332e9fc6611450be9879f5eb1a93c887c`
- Test commit: `9879c60332e9fc6611450be9879f5eb1a93c887c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27 to 27 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 89.14 | 32 | 27 | 7 | 6 | [run](https://argusic.com/run/7b1282bb-5ebb-4cad-ad43-5bca7cc51564) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No PHP runtime pre-installed in container`
- 2 min: `No Composer pre-installed`
- 5 min: `No MySQL server available (no root, no Docker)`
- 3 min: `intl extension (NumberFormatter) not in the common PHP build`
- 5 min: `SQLite doesn't support ANSI OFFSET...FETCH NEXT syntax`
- 2 min: `vendor/aimeos/aimeos-core/Setup.php missing sqlite driver mapping`
- `7 out of 8 Base tests pass; 2 need database tables with seed data; all command/controller tests need a populated MySQL database`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
