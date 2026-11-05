# webmagic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/code4craft/webmagic, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/webmagic

## Pinned environment

- Project commit: `67816a19d68a4fec4657bf1336227e046e251df2`
- Test commit: `67816a19d68a4fec4657bf1336227e046e251df2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 13.5 to 41.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 41.1 | 2 | 2 | [run](https://argusic.com/run/9da5e8a3-dcee-4aa2-a139-e315a89274d6) |
| 2 | pass | 100 | 11 | 13.5 | 1 | 1 | [run](https://argusic.com/run/922f65c6-0988-45a5-a283-b9ebb6d4ddf4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `JDK 11 not installed in container. Install via apt fails due to no root.`
- 2 min: `Maven not installed in container.`

Attempt 2:

- 3 min: `Java 22+ module system blocks mockito-all (cglib) from accessing java.lang.ClassLoader.defineClass, causing ExceptionInInitializerError in 3 tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
