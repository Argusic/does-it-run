# sqlancer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sqlancer/sqlancer, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/sqlancer

## Pinned environment

- Project commit: `9eb1db82e16f1ece0470cc9f424eaf8ba7809e21`
- Test commit: `9eb1db82e16f1ece0470cc9f424eaf8ba7809e21`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 38.8 to 40.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 40.5 | 4 | 4 | [run](https://argusic.com/run/e23ef960-f1b1-4a8f-9ac8-9b1b06b3dad2) |
| 2 | pass | 100 | 38 | 38.8 | 4 | 4 | [run](https://argusic.com/run/721dfc6d-c724-4a46-98a3-274b937ff0b5) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `Java 17+ and Maven not pre-installed in container. Manually downloaded JDK 17 (Temurin) and Maven 3.9.16 from Apache mirrors, extracted to $HOME/tools`
- 1 min: `SQLite3 CLI not installed. SQLancer requires sqlite3 binary to test SQLite (uses it via JDBC driver but the system sqlite3 wasn't present for CLI testing)`
- 3 min: `TestUsageNamingConvention.testNonEmptyDescription failed with InaccessibleObjectException on JDK 17 due to Java module system restrictions`
- `org.glassfish:javax.el Maven metadata couldn't be downloaded from java.net repos due to PKIX certificate path validation failure`

Attempt 2:

- 18 min: `Java 11+ and Maven not pre-installed in container`
- 15 min: `First Maven 3.9.16 download from dlcdn incomplete (lib/ missing most JARs)`
- 2 min: `Maven 3.9.9/3.8.8 URLs on dlcdn.apache.org returned 404`
- `PKIX cert warnings for maven.java.net repos (non-blocking)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
