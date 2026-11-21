# zerocode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/authorjapps/zerocode, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/zerocode

## Pinned environment

- Project commit: `d6694c4a742cda68e60f5cbc858609c255f448d3`
- Test commit: `d6694c4a742cda68e60f5cbc858609c255f448d3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.3 to 64.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 14.3 | 4 | 4 | [run](https://argusic.com/run/de7428df-281e-4100-93b1-580e90a47f75) |
| 2 | pass | 100 | 64 | 64.3 | 4 | 4 | [run](https://argusic.com/run/5f71111d-742f-4725-b5f6-e29f82becaf5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Java or Maven in container`
- 1 min: `TokenUtilsTest.testAbsolutePathOf fails on this machine because it expects path containing 'zerocode/core/target/test-classes/...'`
- 1 min: `DbSqlExecutorScenarioPostgresTest (2 tests) fail - require running PostgreSQL Docker container`
- 1 min: `Inner classes of ZeroCodeLoadRunnerTest/ZeroCodeMultiLoadRunnerTest picked up by Surefire as test classes, causing 7 'initializationError' failures`

Attempt 2:

- 10 min: `testEnvValue: JAVA_HOME env var not set, made test fail`
- 5 min: `testAbsolutePathOf: assertion expected 'zerocode/core/target/...' but actual path is '/work/repo/core/target/...'`
- 5 min: `DbSqlExecutorScenarioPostgresTest x2: no PostgreSQL server available`
- 20 min: `Port conflict (BindException): stale simulator processes and incorrect static state between port 9997/9998 runners`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
