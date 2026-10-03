# orientdb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/orientechnologies/orientdb, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/orientdb

## Pinned environment

- Project commit: `22eaaf9ee01e81a492b6f4a43802c86db82e5c2d`
- Test commit: `22eaaf9ee01e81a492b6f4a43802c86db82e5c2d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 50.4 to 52.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 50 | 50.4 | 3 | 3 | [run](https://argusic.com/run/54702197-b688-4aa7-b7ea-317805723561) |
| 2 | pass | 100 | 12 | 52.4 | 3 | 3 | [run](https://argusic.com/run/d3ce8da1-ad2e-4d54-9538-1b2f4848b916) |
| 3 | pass | 100 | 5 | 51.1 | 2 | 2 | [run](https://argusic.com/run/3ca339a5-0fc2-4423-94d2-df263d5aae8e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Java (JDK) not installed in the container`
- `Maven wrapper needed downloading and running; no local Maven`
- 2 min: `Server startup failed without ORIENTDB_ROOT_PASSWORD env var (null root password)`

Attempt 2:

- `No Java JDK in container - had to download Adoptium Temurin JDK 17 manually`
- `Server tests had 12 HTTP errors (HttpCommandTest, HttpDatabaseTest, etc.) because HTTP endpoints require a running server`
- `Missing config files (custom-sql-functions.json, default-distributed-db-config.json) caused server startup failure on first attempt`

Attempt 3:

- 2 min: `No Java JDK was installed in the container (no apt install possible without root)`
- 2 min: `Initial server launch via manual classpath failed with IllegalAccessError on OServerConfiguration.properties (orientdb-tools jar missing from classpath)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
