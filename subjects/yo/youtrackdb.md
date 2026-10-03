# youtrackdb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JetBrains/youtrackdb, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/youtrackdb

## Pinned environment

- Project commit: `4c875a0f195bcf77394651e0f31df2ece04d8786`
- Test commit: `4c875a0f195bcf77394651e0f31df2ece04d8786`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 62.8 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/54ed34cb-bb58-49a6-8692-dc835befb3d6) |
| 2 | pass | 100 | 20 | 62.8 | 2 | 2 | [run](https://argusic.com/run/fdff1d0f-1b00-4ef9-84a3-9cbcd1f4ab36) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `JDK 21 not pre-installed on the system`
- 1 min: `spotless-maven-plugin required a baseline reference that does not exist (No such reference 'spotless-baseline')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
