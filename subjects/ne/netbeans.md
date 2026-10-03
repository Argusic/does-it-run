# netbeans

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/netbeans, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/netbeans

## Pinned environment

- Project commit: `4d2a85c0e27052ba3f66a868748b7e93859a6fb6`
- Test commit: `4d2a85c0e27052ba3f66a868748b7e93859a6fb6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 30.8 to 30.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 30.8 | 2 | 2 | [run](https://argusic.com/run/477a7c2b-634f-4e56-ac2a-60485d8a7517) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `JDK 21+ not installed in container`
- 1 min: `Apache Ant not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
