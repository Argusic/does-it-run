# objectbox-java

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/objectbox/objectbox-java, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/objectbox-java

## Pinned environment

- Project commit: `e912fe3281925d22276f52bbd84e506d0429a8ae`
- Test commit: `e912fe3281925d22276f52bbd84e506d0429a8ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 9.1 to 13.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 13.5 | 3 | 3 | [run](https://argusic.com/run/02584933-4cc2-42e2-b046-da474dd0cfb9) |
| 2 | pass | 100 | 15 | 9.1 | 2 | 2 | [run](https://argusic.com/run/ab40693e-d2fa-4cdd-b3ad-30dd5b37fe52) |
| 3 | pass | 100 | 8 | 10.3 | 2 | 2 | [run](https://argusic.com/run/f04e8eff-8c7a-46c5-9df5-de01829244f9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No JDK installed in container`
- 3 min: `Snapshot native dependencies not found on Maven Central (need internal GitLab)`
- 1 min: `SpotBugs static analysis exits with code 1`

Attempt 2:

- 2 min: `No Java runtime found in the container; JAVA_HOME not set and 'java' command not in PATH`
- 1 min: `Cannot resolve io.objectbox:objectbox-sync-linux:6.0.0-beta-sync-SNAPSHOT; snapshot-only native libs require internal GitLab repo credentials`

Attempt 3:

- 2 min: `No JDK available in the container (Gradle 9.5.1 requires JVM 17+)`
- 1 min: `Snapshot dependencies (objectbox-sync-*:6.0.0-beta-sync-SNAPSHOT) unavailable because the internal GitLab repository was not configured`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
