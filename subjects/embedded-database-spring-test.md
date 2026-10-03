# embedded-database-spring-test

**Verdict: runs.** Argusic Score 93.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zonkyio/embedded-database-spring-test, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/embedded-database-spring-test

## Pinned environment

- Project commit: `78158b2dfa12976afcfb4a42c8c2c613fc82bf57`
- Test commit: `78158b2dfa12976afcfb4a42c8c2c613fc82bf57`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 24.8 to 25.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 25.5 | 3 | 3 | [run](https://argusic.com/run/40b6cfba-f091-4b55-9797-81ff71f34c2a) |
| 2 | pass with mocks | 87 | 24 | 24.8 | 4 | 3 | [run](https://argusic.com/run/0679bc21-ba57-4329-9660-467f153e560e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No JDK found in container`
- 5 min: `Docker daemon unavailable; tests defaulting to Docker provider failed`
- 2 min: `Initdb locale 'cs_CZ.UTF-8' not available in container (only C, C.utf8, POSIX)`

Attempt 2:

- 1 min: `Gradle wrapper 7.3.3 incompatible with JDK 21 (Unsupported class file major version 65)`
- 1 min: `cs_CZ.UTF-8 locale unavailable in container; initdb fails when tests set lc-collate=cs_CZ.UTF-8`
- 1 min: `Tests hardcode dockerPostgresDatabaseProvider bean name, incompatible with embedded provider`
- `Docker socket unavailable; 14 Docker-dependent tests cannot run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
