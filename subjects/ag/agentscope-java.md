# agentscope-java

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agentscope-ai/agentscope-java, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/agentscope-java

## Pinned environment

- Project commit: `857e3e6cf1af09abb5a422f882635c3f15f82e34`
- Test commit: `857e3e6cf1af09abb5a422f882635c3f15f82e34`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 79 to 79 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 79 | 3 | 3 | [run](https://argusic.com/run/3444116c-b127-4e13-b0e3-fcea866d18af) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `JDK 17 not pre-installed in container`
- 2 min: `Maven not pre-installed in container`
- 0.5 min: `Maven tarball truncated on first download attempt`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
