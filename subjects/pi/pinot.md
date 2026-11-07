# pinot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/pinot, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/pinot

## Pinned environment

- Project commit: `0a53497fddfc61220feabc5b8f62516f4183525f`
- Test commit: `0a53497fddfc61220feabc5b8f62516f4183525f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 25.6 to 61.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 25.6 | 0 | 0 | [run](https://argusic.com/run/36255f17-3a85-44ec-bfbd-f563dae61dbd) |
| 2 | pass | 100 | 32 | 61.5 | 4 | 4 | [run](https://argusic.com/run/ba7eebf0-fb68-4aae-8bd3-73c5ba72ef6c) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `No JDK installed in container (JAVA_HOME not set, mvnw cannot run); system packages cannot be installed without root`
- 12 min: `Maven build failed twice with 'Java heap space' OOM while compiling pinot-minion and packaging pinot-tools under 1GB container memory`
- 9 min: `Test run 'mvn -pl pinot-segment-local -am -Dtest=RangeIndexTest -Dsurefire.failIfNoSpecifiedTests=false test' ends with MojoFailureException: TestNG engine (auto-added via surefire junit-platform provider) executes a phantom empty suite and`
- 2 min: `First offline test attempt failed because -o blocked downloading surefire-junit-platform provider jar; no repo-level fix possible while offline`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
