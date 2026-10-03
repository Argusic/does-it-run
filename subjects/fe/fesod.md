# fesod

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/fesod, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/fesod

## Pinned environment

- Project commit: `c9e68133c583afa002bc6220aa9b94d85889ceca`
- Test commit: `c9e68133c583afa002bc6220aa9b94d85889ceca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 4.8 to 30.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 9.3 | 2 | 2 | [run](https://argusic.com/run/eb268d34-7629-404b-90ea-c8da709d167f) |
| 2 | pass | 100 | 3 | 4.8 | 1 | 1 | [run](https://argusic.com/run/15a03a35-36ba-4688-8968-0744b203c3b6) |
| 3 | pass | 100 | 29 | 30.8 | 2 | 2 | [run](https://argusic.com/run/fab25313-dcc7-42c5-a7f8-10cf8b67c2b1) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No JDK found in container`
- 4 min: `Maven test lifecycle skips shade plugin, causing missing cglib packages in fesod-sheet compilation`

Attempt 2:

- 0.5 min: `java: not found , no JDK in container`

Attempt 3:

- 5 min: `JDK not installed in container`
- 9 min: `mvnw wrapper downloaded Maven and all dependencies from Maven Central`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
