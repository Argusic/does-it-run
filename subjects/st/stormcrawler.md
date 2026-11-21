# stormcrawler

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/stormcrawler, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/stormcrawler

## Pinned environment

- Project commit: `e94fed1efbaf93fb665ca186cd161261922d6ca0`
- Test commit: `e94fed1efbaf93fb665ca186cd161261922d6ca0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.3 to 19.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 15.3 | 2 | 2 | [run](https://argusic.com/run/759a6fe5-7509-45c3-a669-4b7831efa45d) |
| 2 | pass | 100 | 14 | 19.8 | 5 | 5 | [run](https://argusic.com/run/f6b0de80-c4a0-4398-ae33-50612857fd0e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Java runtime found in container`
- 1 min: `No Maven found in container`

Attempt 2:

- 2 min: `Java and Maven not pre-installed in container`
- 2 min: `JDK 25 deb symlinks to /etc/java-25-openjdk/ were dangling (no /etc dir from dpkg-deb -x)`
- 5 min: `JDK 25 PKCS12 trust store empty / SSL trustAnchors InvalidAlgorithmParameterException`
- 1 min: `Maven 3.8.7 Debian package had broken symlinks to separate libmaven3-core-java package`
- 1 min: `Test-jar missing for stormcrawler-core dependency in downstream modules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
