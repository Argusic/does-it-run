# logbook

**Verdict: runs.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zalando/logbook, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/logbook

## Pinned environment

- Project commit: `f4f1e6372f449c193e5eb2a21478d07ef766c2a3`
- Test commit: `f4f1e6372f449c193e5eb2a21478d07ef766c2a3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 0.9 to 20 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.4 | 20 | 0 | 0 | [run](https://argusic.com/run/7df0dad3-f2d3-4f1b-aaf8-93c02cdcfc1b) |
| 2 | fail | 0 | 0 | 0.9 | 1 | 0 | [run](https://argusic.com/run/56390ce8-d4f5-4440-a73d-49044a053417) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Java 17+ is not installed in the container and cannot be installed (no root access, no SDKMAN, no pre-installed JDK). The Maven wrapper (mvnw) requires JAVA_HOME which is not set.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
