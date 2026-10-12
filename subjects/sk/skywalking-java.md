# skywalking-java

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/skywalking-java, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/skywalking-java

## Pinned environment

- Project commit: `7f681f72148e138365b80c05dbb7d14d3c93ba84`
- Test commit: `7f681f72148e138365b80c05dbb7d14d3c93ba84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 42.7 to 42.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 48 | 42.7 | 4 | 4 | [run](https://argusic.com/run/d27e7afa-c7e3-4370-a28e-0af424e6bfb2) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `No JDK or Maven installed in container (no root)`
- 1 min: `Proto submodule not initialized at clone`
- 3 min: `mvnw test -pl apm-sniffer/apm-agent-core failed resolving sibling SNAPSHOTs`
- 10 min: `Mock collector harness missing grpc-netty/perfmark/failureaccess on ad-hoc classpath`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
