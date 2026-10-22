# ReplicaDB

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/osalvador/ReplicaDB, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/replicadb

## Pinned environment

- Project commit: `05ef8d468bcbaa633f82f640a0215b49852912b6`
- Test commit: `05ef8d468bcbaa633f82f640a0215b49852912b6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18.4 to 18.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 18.4 | 5 | 5 | [run](https://argusic.com/run/6651ba9c-3eb6-4b6c-b07c-d568d118e54d) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Java JDK 17 not installed`
- 4 min: `Maven not installed`
- 1 min: `Default JAR had no main manifest`
- `Docker unavailable - 500 Testcontainer tests cannot run in CLI module`
- `Docker unavailable - 124 Testcontainer tests cannot run in server module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
