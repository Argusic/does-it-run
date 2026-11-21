# jbake

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jbake-org/jbake, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/jbake

## Pinned environment

- Project commit: `ee32be317336158be567e002744398ef86c89afd`
- Test commit: `ee32be317336158be567e002744398ef86c89afd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.9 to 28.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 7.9 | 0 | 0 | [run](https://argusic.com/run/c7ebd675-b746-4814-99e6-3c35c4e74231) |
| 2 | pass | 100 | 27 | 28.3 | 2 | 2 | [run](https://argusic.com/run/cef973dd-5a3d-4792-b5d5-624b610651f7) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `No JDK installed in container`
- 5 min: `Gradle build cache served stale class files causing test compilation to fail with cannot-find-symbol errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
