# Java

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TheAlgorithms/Java, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/java

## Pinned environment

- Project commit: `2105b5652a541cbf5db0904d0cfebbaf487e4c5f`
- Test commit: `2105b5652a541cbf5db0904d0cfebbaf487e4c5f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 33.9 to 33.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 32 | 33.9 | 2 | 1 | [run](https://argusic.com/run/f1a9dba1-4422-4837-b34d-dba96231ff1c) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Surefire fork mode on JDK 21 caused NoClassDefFoundError for 1355 inner classes (SplayTree$EmptyTreeException, LZ78, UnitConversions, etc.)`
- `LongestCommonSubstringTest: 2 timeout failures (execution timed out after 2000ms on large inputs)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
