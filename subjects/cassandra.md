# cassandra

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/cassandra, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/cassandra

## Pinned environment

- Project commit: `17137ce34bd2fa89bc296e2d61d59eac9957b787`
- Test commit: `17137ce34bd2fa89bc296e2d61d59eac9957b787`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.6 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.6 | 2 | 2 | [run](https://argusic.com/run/dcbd140d-284f-4627-a9e6-b5dfd2be990e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Java JDK installed in environment`
- 1 min: `No Apache Ant installed in environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
