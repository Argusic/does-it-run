# yas

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nashtech-garage/yas, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/yas

## Pinned environment

- Project commit: `179e813568c345bad3fce985088b5535e57481aa`
- Test commit: `179e813568c345bad3fce985088b5535e57481aa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 43.3 to 43.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 42 | 43.3 | 3 | 3 | [run](https://argusic.com/run/4610a852-13ba-4f14-bb20-ce59b0df9064) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `No JDK or Maven installed in container`
- `search module tests fail - Docker Testcontainers require Keycloak and Kafka containers`
- `recommendation module tests fail - Docker Testcontainers require Kafka`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
