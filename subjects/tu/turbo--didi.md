# turbo

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/didi/turbo, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/run/b642facd-a8f6-4021-a85b-b85c2ded6abf

## Pinned environment

- Project commit: `4cac6b00af0f70351b3e3ef5a69527e380ab01e2`
- Test commit: `4cac6b00af0f70351b3e3ef5a69527e380ab01e2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 22.2 to 22.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 22.2 | 2 | 2 | [run](https://argusic.com/run/b642facd-a8f6-4021-a85b-b85c2ded6abf) |
| 2 | pass | 100 | 15 | 22.6 | 7 | 7 | [run](https://argusic.com/run/7c3450a3-9e88-4b14-a1a3-342dafa4f4c1) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Engine JUnit 4 tests skipped (no Vintage Engine), no H2 test config`
- 1 min: `BaseTest had no runnable methods, caused InvalidTestClass error on Surefire`

Attempt 2:

- 1 min: `No JDK available in container - java not found`
- 0.5 min: `No Maven available in container - mvn not found`
- 2 min: `Engine tests configured for MySQL but MySQL is not running`
- 2 min: `Parallel-plugin tests configured for MySQL - same issue`
- 0.5 min: `JUnit version conflict between vintage 5.10.2 and platform 1.12.2`
- 0.5 min: `Abstract BaseTest class detected as runnable test`
- `Parallel-plugin RuntimeProcessorTest: 3/9 tests fail when run in batch due to shared H2 in-memory DB state crossing test boundaries`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
