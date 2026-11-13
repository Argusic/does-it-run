# yas

**Verdict: runs.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nashtech-garage/yas, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/yas

## Pinned environment

- Project commit: `179e813568c345bad3fce985088b5535e57481aa`
- Test commit: `179e813568c345bad3fce985088b5535e57481aa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 39.3 to 43.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 42 | 43.3 | 3 | 3 | [run](https://argusic.com/run/4610a852-13ba-4f14-bb20-ce59b0df9064) |
| 2 | pass with mocks | 72 | 30 | 39.3 | 2 | 0 | [run](https://argusic.com/run/6ca44f30-5b1c-4c88-a353-555096acf486) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `No JDK or Maven installed in container`
- `search module tests fail - Docker Testcontainers require Keycloak and Kafka containers`
- `recommendation module tests fail - Docker Testcontainers require Kafka`

Attempt 2:

- 5 min: `search and recommendation integration tests failed: Testcontainers requires Docker for Keycloak/Kafka/Elasticsearch containers (Could not find a valid Docker environment)`
- 1 min: `automation-ui (Selenium integration suite) requires a running deployment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
