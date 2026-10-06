# elassandra

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/strapdata/elassandra, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/elassandra

## Pinned environment

- Project commit: `b90667791768188a98641be0f758ff7cd9f411f0`
- Test commit: `b90667791768188a98641be0f758ff7cd9f411f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 43.9 to 43.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 43.9 | 2 | 2 | [run](https://argusic.com/run/a182ee23-2dc4-4406-9e46-5d28d30a82b4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Building from source fails: JCenter Maven repo is offline, nebula/p4java dependencies unavailable from Maven Central/Gradle Plugin Portal`
- 1 min: `Container has only 1GB RAM; Cassandra with default 8GB heap gets OOM-killed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
