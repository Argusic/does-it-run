# jenkins-library

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SAP/jenkins-library, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/jenkins-library

## Pinned environment

- Project commit: `7cea829d845a03127a61292ad39add15ed935ab1`
- Test commit: `7cea829d845a03127a61292ad39add15ed935ab1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.4 to 14.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 10 | 14.4 | 2 | 1 | [run](https://argusic.com/run/806b8313-d610-4f94-ab45-a8239117b0ff) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No Go toolchain in container`
- 3 min: `java and mvn not installed, so Groovy library tests cannot run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
