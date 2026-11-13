# AnExplorer

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/1hakr/AnExplorer, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/anexplorer

## Pinned environment

- Project commit: `e856926de57c4e403b8678bf3b289ac618065648`
- Test commit: `e856926de57c4e403b8678bf3b289ac618065648`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 7.2 to 38.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 7.2 | 6 | 6 | [run](https://argusic.com/run/43d05dd0-a2f6-47f3-9825-05d911acec7a) |
| 2 | pass with mocks | 92 | 38 | 38.1 | 8 | 8 | [run](https://argusic.com/run/cb30bf7a-5a87-481c-a955-fda92c2c8b1f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `MaxPermSize JVM option not recognized by JDK 17`
- 1 min: `maven.fabric.io:gradle:1.25.4 returned 403`
- 3 min: `No Android SDK installed`
- 1 min: `JAXB Injector InaccessibleObjectException on JDK 17`
- 1 min: `keystore.properties values interpreted as bare identifiers`
- `ApplicationTest.java cannot find ApplicationTestCase`

Attempt 2:

- 4 min: `No Java installed`
- 4 min: `Dead Fabric dependency (io.fabric.tools:gradle:1.25.4) blocking Gradle config`
- 1 min: `MaxPermSize JVM flag incompatible with JDK 17`
- 5 min: `Android SDK not installed`
- 6 min: `Android Gradle Plugin 3.3.0-alpha12 incompatible with JDK 17 (ExceptionInInitializerError)`
- 4 min: `Dex merge fails due to 64K method reference limit (68,810 > 65,536)`
- 3 min: `SigningConfigs and Fabric references in app/build.gradle blocked build`
- 1 min: `JCenter and maven.fabric.io repos unavailable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
