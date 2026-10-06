# spring-framework

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spring-projects/spring-framework, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/spring-framework

## Pinned environment

- Project commit: `9b93e5f635dd6576cf049f8e1f8f623968c88047`
- Test commit: `9b93e5f635dd6576cf049f8e1f8f623968c88047`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 10 | 1 | 1 | [run](https://argusic.com/run/e5b5c92f-901f-413b-a377-d785b9a21cd6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `JAVA_HOME is not set and no java command found in PATH. Project requires JDK 25 (per .sdkmanrc) but container had no JDK installed.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
