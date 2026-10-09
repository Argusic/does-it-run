# infinispan

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/infinispan/infinispan, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/infinispan

## Pinned environment

- Project commit: `cc2008fd81477ef9aa615a53c385d22fd9036753`
- Test commit: `cc2008fd81477ef9aa615a53c385d22fd9036753`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.5 to 20.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 20.5 | 2 | 2 | [run](https://argusic.com/run/67e1027b-d874-4573-911f-77cf4b0521ff) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `JDK not installed on system. POM enforcer requires JDK 25.`
- 2 min: `First download JDK 21 but enforcer rule [25,) rejected it.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
