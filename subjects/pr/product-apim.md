# product-apim

**Verdict: runs.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wso2/product-apim, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/product-apim

## Pinned environment

- Project commit: `9e253b10599cdb5824f1773f3b79395987821b1a`
- Test commit: `9e253b10599cdb5824f1773f3b79395987821b1a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 2.9 to 67.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 0 | 2.9 | 3 | 0 | [run](https://argusic.com/run/95e15281-c5cf-46fc-b68b-254d04a30914) |
| 2 | pass | 100 | 66 | 67.3 | 3 | 3 | [run](https://argusic.com/run/2ac7bb17-190c-4226-b7be-f8b0a1b6f6ad) |

## What was observed on a clean machine

Attempt 1:

- `No JDK 21 or JRE installed on system. Java is required for this Maven-based Java project (WSO2 API Manager).`
- `No Maven installed. Project uses Maven multi-module build (pom.xml at root and in 4 sub-projects).`
- `No root access to install packages via apt. No network download capability to fetch portable JDK/Maven.`

Attempt 2:

- 2 min: `JDK 21 not found on system - JAVA_HOME unset, no JDK anywhere in filesystem`
- 2 min: `Maven not found on system - mvn command not available`
- `unzip command not available for extracting archives`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
