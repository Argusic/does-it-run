# diboot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dibo-software/diboot, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/diboot

## Pinned environment

- Project commit: `cd211a2dcc067491f199e3a298e43c3dcabf2a25`
- Test commit: `cd211a2dcc067491f199e3a298e43c3dcabf2a25`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 38.5 to 44.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 38.5 | 7 | 7 | [run](https://argusic.com/run/2c985b1c-f8b6-4840-a5dd-30a9b93201c8) |
| 2 | pass | 100 | 12 | 44.7 | 4 | 4 | [run](https://argusic.com/run/e0201c94-702e-48eb-b8a1-a52052672dbb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No JDK pre-installed in container`
- 2 min: `No Maven pre-installed in container`
- 8 min: `No MySQL-compatible database available`
- 2 min: `MariaDB client binary libncurses.so.5 not found`
- 5 min: `MariaDB process died when parent shell exited`
- 3 min: `mysql-connector-python default collation utf8mb4_0900_ai_ci not supported by MariaDB 11.4`
- 3 min: `Root user auth failed via TCP on fresh MariaDB install due to unix_socket auth plugin`

Attempt 2:

- 2 min: `Java and Maven not pre-installed`
- 1 min: `rest-api-example failed to compile: FileAccessInterceptor not found`
- 2 min: `JUnit4 tests not detected by Surefire (only JUnit Platform provider)`
- 5 min: `Tests require MySQL on port 3307`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
