# spring-cloud-gateway

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spring-cloud/spring-cloud-gateway, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/spring-cloud-gateway

## Pinned environment

- Project commit: `88a92c065767a20a5d37753437d15975a8c06c28`
- Test commit: `88a92c065767a20a5d37753437d15975a8c06c28`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 68.6 to 68.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 68.6 | 3 | 3 | [run](https://argusic.com/run/4265adc7-0d18-4625-94be-04161fbe1970) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Java JDK found in container`
- 4 min: `StreamRoutingFilterTests uses Testcontainers (RabbitMQ) but lacks @Tag("DockerRequired"), causing container fetch error`
- 2 min: `All 19 WebMVC test classes use HttpbinTestcontainers requiring Docker, causing 105 test errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
