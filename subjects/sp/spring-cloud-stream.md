# spring-cloud-stream

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spring-cloud/spring-cloud-stream, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/spring-cloud-stream

## Pinned environment

- Project commit: `4d7cce1b276112ec3c8fdc0d8fe21c46b7acd283`
- Test commit: `4d7cce1b276112ec3c8fdc0d8fe21c46b7acd283`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 61.9 to 61.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 61 | 61.9 | 4 | 4 | [run](https://argusic.com/run/6e68a156-d82c-4dbe-bf84-d389af0965cd) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No JDK or Maven present in container; downloaded user-space Temurin JDK 17 and Maven 3.9.9 to ~/tools`
- 18 min: `mvn test on spring-cloud-stream-binder-rabbit failed: Testcontainers RabbitTestContainer requires a Docker daemon (Could not find a valid Docker environment); Docker cannot be installed here (no root, no newuidmap/slirp4netns, no docker soc`
- 10 min: `No system packages can be installed (no root); Erlang asn1 app initially missing from extracted tree`
- 5 min: `mvn install for the Rabbit binder module has no external-broker env switch (test harness hard-wires org.testcontainers.containers.RabbitMQContainer static init), so that module suite cannot run without Docker`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
