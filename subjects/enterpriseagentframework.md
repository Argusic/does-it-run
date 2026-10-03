# EnterpriseAgentFramework

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/w8123/EnterpriseAgentFramework, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/enterpriseagentframework

## Pinned environment

- Project commit: `ea9c782da5904858b30b87be422a2d0cc390c4ab`
- Test commit: `ea9c782da5904858b30b87be422a2d0cc390c4ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 22.6 to 33.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 22.6 | 3 | 3 | [run](https://argusic.com/run/c3dc415d-e7b3-4c98-8af6-6d0256753951) |
| 2 | pass | 100 | 33 | 33.7 | 2 | 2 | [run](https://argusic.com/run/03add6fb-9deb-492f-806f-1f991800b42f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `reachai-capability-sdk and reachai-spring-boot2-starter JAR files missing from control-service classpath resources`
- 1 min: `SHA-256 checksum files in java-sdk artifacts didn't match the actual built JARs/POMs`
- 3 min: `AiCodingTaskProtocolHttpTest.generatedWindowsBootstrapRestoresEncryptedSessionAndWritesUtf8Artifact NPE on Linux: System.getenv(SystemRoot) is null`

Attempt 2:

- 2 min: `Missing Java SDK JAR artifacts in classpath resources directory reachai-control-service/src/main/resources/ai-assist/artifacts/java-sdk/`
- 2 min: `NullPointerException in AiCodingTaskProtocolHttpTest.generatedWindowsBootstrapRestoresEncryptedSessionAndWritesUtf8Artifact: System.getenv("SystemRoot") returns null on Linux before assumeTrue guard`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
