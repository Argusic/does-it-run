# nitrite-java

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nitrite/nitrite-java, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/nitrite-java

## Pinned environment

- Project commit: `b3ca3d68287e20c06bf743e0aee8cfbd7f8aa1bf`
- Test commit: `b3ca3d68287e20c06bf743e0aee8cfbd7f8aa1bf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 26.7 to 44.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 44.6 | 0 | 0 | [run](https://argusic.com/run/d77fb795-a45c-4a27-8772-f4c82d1b5636) |
| 2 | pass | 100 | 2 | 26.7 | 2 | 2 | [run](https://argusic.com/run/4c4090c2-4e14-4c60-a0f0-155a4540ec67) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `JDK 11 cannot compile Jackson 3.2.2 (class version 61.0, requires Java 17)`
- 1 min: `Maven 3.9.9 download returned 404 from dlcdn.apache.org`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
