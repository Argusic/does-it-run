# zeppelin

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/zeppelin, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/zeppelin

## Pinned environment

- Project commit: `703fe6763f6f5aefbe66004327579d8b6cfd95e6`
- Test commit: `703fe6763f6f5aefbe66004327579d8b6cfd95e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 36.9 to 72.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 36.9 | 3 | 3 | [run](https://argusic.com/run/af8db605-c262-461a-8dd3-94ea42c8fee8) |
| 2 | pass with mocks | 92 | 33 | 72.7 | 3 | 3 | [run](https://argusic.com/run/016fbedf-163c-4469-82d9-34daf30a4fa3) |
| 3 | pass | 100 | 54 | 55.1 | 5 | 5 | [run](https://argusic.com/run/75056288-e545-494a-9e83-60af2c57d4b5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No JDK installed in container`
- 5 min: `Server integration tests need pre-built interpreter directories`
- 1 min: `copy-dependencies fails on reactor artifacts when using test without prior package`

Attempt 2:

- 2 min: `JAVA_HOME not set; no JDK on system`
- 8 min: `Test NotebookRestApiTest, ZeppelinRestApiTest, SparkInterpreterLauncherTest failed for missing ../interpreter/sh and ../interpreter/spark/scala-2.12 directories`
- `Full zeppelin-server test suite took >10 min with hanging interpreter JVMs`

Attempt 3:

- 1 min: `JDK 11 not installed in container (no java binary found)`
- 2 min: `zeppelin-web-angular npm postinstall fails: 'playwright install --with-deps' needs root for system dependencies`
- 0.5 min: `zeppelin-distribution depends on zeppelin-web-angular WAR which was skipped`
- 0.5 min: `Lucene write.lock from previous server run blocks new start`
- 0.5 min: `python command not found (only python3 available), causing NotebookRestApiTest to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
