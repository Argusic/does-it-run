# erupt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/erupts/erupt, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/erupt

## Pinned environment

- Project commit: `0e83df6e42dab8b64f19e1670d9b470d252187ab`
- Test commit: `0e83df6e42dab8b64f19e1670d9b470d252187ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.4 to 25.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 25.4 | 2 | 2 | [run](https://argusic.com/run/9f75d07a-9f8a-49e7-8689-88aa9ec419d0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Java cacerts keystore was in PKCS12 format but JVM TLS layer requires JKS format`
- 1 min: `spring-boot-maven-plugin was commented out in erupt-sample/pom.xml, blocking mvn spring-boot:run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
