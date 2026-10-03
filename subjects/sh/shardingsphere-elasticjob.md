# shardingsphere-elasticjob

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/shardingsphere-elasticjob, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/shardingsphere-elasticjob

## Pinned environment

- Project commit: `2a747ab788f9ff0c1cde0d123cd7206bba480531`
- Test commit: `2a747ab788f9ff0c1cde0d123cd7206bba480531`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.6 to 19.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 19.6 | 3 | 3 | [run](https://argusic.com/run/5a47addd-bab6-45f4-84d1-e564b300d22b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No JDK installed in container - Java 8+ required`
- 1 min: `No ZooKeeper installed - ZooKeeper 3.6+ required`
- 1 min: `JDK 11 rejected by maven-enforcer-plugin - requires JDK 17+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
