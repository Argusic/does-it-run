# conductor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/conductor-oss/conductor, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/conductor

## Pinned environment

- Project commit: `da325130588fdff8ed89f924d77a970ca63bcdf1`
- Test commit: `da325130588fdff8ed89f924d77a970ca63bcdf1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.4 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 13.4 | 4 | 4 | [run](https://argusic.com/run/ef0e7464-de0c-4f50-9c19-64b68ffa8221) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Java 21 not installed in container. No package manager access (no root).`
- 1 min: `npm install -g failed: EACCES writing to /usr/local/lib/node_modules (no root).`
- 1 min: `conductor workflow create failed: no server configured (CONDUCTOR_SERVER_URL not set by conductor server start).`
- 3 min: `2 failing tests in conductor-ai module: MongoVectorDBTest and JDBCEndToEndTest require Docker, which is unavailable in this container.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
