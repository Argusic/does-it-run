# zipkin

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openzipkin/zipkin, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/zipkin

## Pinned environment

- Project commit: `878ce2a1fad54ca941d17fdcf2e1d924b148eb1f`
- Test commit: `878ce2a1fad54ca941d17fdcf2e1d924b148eb1f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.1 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 8.1 | 3 | 3 | [run](https://argusic.com/run/bf3fb060-f562-4c1a-b70a-de4aed5ca3be) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No JDK found in container`
- 1 min: `JDK 17 rejected by maven-enforcer (requires [21,22))`
- `Server process died when shell command exited`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
