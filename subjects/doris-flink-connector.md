# doris-flink-connector

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/doris-flink-connector, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/doris-flink-connector

## Pinned environment

- Project commit: `b5f65fb98efbfa1efafb553b6bec9bfab853754f`
- Test commit: `b5f65fb98efbfa1efafb553b6bec9bfab853754f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.8 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.5 | 3 | 3 | [run](https://argusic.com/run/088810c9-53bf-4867-9628-ad69f312f616) |
| 2 | pass | 93.33 | 1.5 | 6.8 | 3 | 2 | [run](https://argusic.com/run/b667ecab-39bc-4318-9a96-7b277e81ba06) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No JDK 17 installed in container`
- `No standalone Maven installed`
- 1 min: `flink2 module could not resolve flink-doris-connector-base as sibling dependency`

Attempt 2:

- 1 min: `No JDK or Maven available in container`
- 0.5 min: `Missing test-jar dependency for flink-doris-connector-base`
- `IT module has pre-existing Guava shading compilation error in DorisRowDataJdbcLookupFunctionITCase.java`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
