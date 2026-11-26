# scalardb

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/scalar-labs/scalardb, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/scalardb

## Pinned environment

- Project commit: `7e13e0e31851ec1a3632b424a6bb031cdb67fb11`
- Test commit: `7e13e0e31851ec1a3632b424a6bb031cdb67fb11`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 17.3 to 27 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 17.3 | 1 | 1 | [run](https://argusic.com/run/98532274-2d00-44e9-8ba6-9b8b66d05aa6) |
| 2 | pass | 100 | 27 | 27 | 4 | 4 | [run](https://argusic.com/run/dd953872-8bd4-4196-940b-4144ce77ac25) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `ConfigUtilsTest.trimAndReplace_ShouldBehaveCorrectly failed on Java 17+ due to system-lambda library using reflection on java.util.Collections which is blocked by Java modules`

Attempt 2:

- 2 min: `No JDK in environment: JAVA_HOME unset, no java binary found`
- 1 min: `Javadoc generation failed: 3 heading-order errors in javadoc comments`
- 1 min: `ConfigUtilsTest failure: stefanbirkner SystemLambda reflection blocked by Java 17 module system`
- 1 min: `SpotBugs check failed: EI_EXPOSE_REP in KeyBytesEncoder`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
