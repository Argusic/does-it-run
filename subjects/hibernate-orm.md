# hibernate-orm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hibernate/hibernate-orm, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/hibernate-orm

## Pinned environment

- Project commit: `e1f9fc665890067291278b67d3356b1e6754e554`
- Test commit: `e1f9fc665890067291278b67d3356b1e6754e554`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.4 to 24.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 24.4 | 3 | 3 | [run](https://argusic.com/run/e1751342-ca89-4ada-b1ce-2a8c605a3b8f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No JDK installed in container`
- 1 min: `unzip not available (no root access), blocking SDKMAN install`
- `Gradle daemon worker shutdown race at end of test run (Could not stop all services)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
