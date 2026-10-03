# hertzbeat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/hertzbeat, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/hertzbeat

## Pinned environment

- Project commit: `d5995a9675117568d6cad7241bb663ddb620dba0`
- Test commit: `d5995a9675117568d6cad7241bb663ddb620dba0`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 23 to 86.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23.4 | 23 | 2 | 2 | [run](https://argusic.com/run/506614f5-b9fd-49e8-996f-8629acd7c1ca) |
| 2 | pass | 100 | 6.2 | 86.1 | 5 | 5 | [run](https://argusic.com/run/959095ee-168c-4a49-8354-9e3ed4a9f6f1) |
| 3 | pass | 100 | 12 | 37.4 | 3 | 3 | [run](https://argusic.com/run/2f68f040-271c-4efc-882a-517e4ca8446c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Java 25 and Maven not preinstalled`
- 2 min: `Maven 3.9.9 download URL returned 404`

Attempt 2:

- 2.5 min: `JDK 17 installed initially, but project requires JDK 25+`
- 1 min: `Maven not pre-installed`
- 0.5 min: `Maven checkstyle plugin XML parse error on 'compile' phase`
- 0.5 min: `H2 database file locking between test runs caused ApplicationContext failures in dao tests`
- 0.5 min: `StartupMysqlR2dbcCompatibilityTest requires Docker for Testcontainers`

Attempt 3:

- 5 min: `No java/mvn in container and no root: README requires java25 + maven3+. Downloaded Temurin JDK 25.0.4.1 and Maven 3.9.9 to ~/tools and set JAVA_HOME/PATH.`
- 31 min: `mvn test: StartupMysqlR2dbcCompatibilityTest requires Testcontainers Docker (spins up mysql:8.0.36); no docker/podman/dockerd socket and no root, so no mock can be stood up in this container.`
- 20 min: `Plain 'java -jar apache-hertzbeat-1.9.0.jar' fails with NoClassDefFoundError: SpringApplication; package must be built via -Prelease and launched with classpath lib/* + main class.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
