# slothdb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SouravRoy-ETL/slothdb, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/slothdb

## Pinned environment

- Project commit: `8180f215847015944c935f56f008d194e2c1494c`
- Test commit: `8180f215847015944c935f56f008d194e2c1494c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.1 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 12.1 | 2 | 2 | [run](https://argusic.com/run/c41318b5-19ee-4659-9db7-d2cd56d88dad) |
| 2 | pass | 100 | 12 | 13.4 | 4 | 4 | [run](https://argusic.com/run/4137b792-544b-42a6-87c6-19323b29e055) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `STRFTIME(t) with 1 arg segfaults , executor dereferences expr.arguments[1] without bounds check`
- 5 min: `7 test failures in LAST_DAY, MAKE_DATE, and CURRENT_DATE , tests expected YYYYMMDD int32 encoding / microsecond timestamps, but engine stores DATE as days-since-epoch int32`

Attempt 2:

- 2 min: `STRFTIME test segfault: test called STRFTIME(t) with 1 arg but executor requires a format string as 2nd arg (expr.arguments[1])`
- 2 min: `LAST_DAY tests failed: executor now returns DATE (epoch days as int32) but tests expected int64 microseconds`
- 2 min: `MAKE_DATE tests failed: executor now returns DATE (epoch days) but tests expected YYYYMMDD integer`
- 1 min: `CURRENT_DATE test failed: executor now returns DATE (epoch days) but test expected YYYYMMDD`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
