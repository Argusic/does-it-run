# jmxterm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jiaqi/jmxterm, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/jmxterm

## Pinned environment

- Project commit: `ab8b84981a5c443833a4dcc14197def958fab69d`
- Test commit: `ab8b84981a5c443833a4dcc14197def958fab69d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.1 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.1 | 1 | 1 | [run](https://argusic.com/run/c99773a3-b0e1-45a3-b0a3-de82d2a0d200) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `fmt-maven-plugin:2.29 requires Java 17 but project default JDK 11 was installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
