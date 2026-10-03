# feign

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenFeign/feign, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/feign

## Pinned environment

- Project commit: `8c719937ae5f059177024235b491a71bf405f2ff`
- Test commit: `8c719937ae5f059177024235b491a71bf405f2ff`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 32 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 10 | 87.1 | 3 | 3 | [run](https://argusic.com/run/4eb5f1e3-1705-4c99-ac6d-96e5ba18ab92) |
| 2 | pass with mocks | 92 | 32 | 32 | 6 | 6 | [run](https://argusic.com/run/71e86a14-5d64-449c-8c29-7719ef402f8a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `'.mvn/jvm.config' contained '--sun-misc-unsafe-memory-access=allow' which is only supported on JDK 22+`
- 3 min: `No Maven toolchains.xml configured , build failed with 'Cannot find matching toolchain' for JDK 1.8 and 25`
- 30 min: `Develocity extension in .mvn/extensions.xml triggers Kotlin daemon that hangs multi-module builds in memory-constrained environments`

Attempt 2:

- 4 min: `No JDK available in container`
- 3 min: `mvnw wrapper uses mvnd 1.0.6 which requires JDK 22+ (--sun-misc-unsafe-memory-access=allow)`
- 1 min: `toolchains.xml missing JDK 1.8 definition required by maven-toolchains-plugin`
- 1 min: `testCompile target release 25 exceeds JDK 21 capability`
- 2 min: `Test code uses unnamed variables (Java 21 preview feature) but --enable-preview not set for compilation or runtime`
- 2 min: `16 test files use java.io.IO.println() (Java 22+ preview class) not present in JDK 21`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
