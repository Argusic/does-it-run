# tinystruct

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tinystruct/tinystruct, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/tinystruct

## Pinned environment

- Project commit: `8efb3a9b26f89bd732f4108835d779c0f8e78b20`
- Test commit: `8efb3a9b26f89bd732f4108835d779c0f8e78b20`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.4 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 17.4 | 4 | 4 | [run](https://argusic.com/run/7e936693-9abf-414d-852c-a7b708e50952) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Java JDK 17+ installed in the container`
- 2 min: `ActionTests.testAction:44 expected 'CST' date format but JVM timezone was UTC`
- 1 min: `JWTManagerTest.testTokenWithClockSkew:88 token with 0h validity expired immediately with 0 clock skew (system already in UTC)`
- 1 min: `java.awt.Desktop.browse throws UnsupportedOperationException in headless environment on server start (Thread-2)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
