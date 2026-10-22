# sdk-java

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/temporalio/sdk-java, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/sdk-java

## Pinned environment

- Project commit: `8d2f35e7d90d21e9d5ae8551e3202e891701bc4a`
- Test commit: `8d2f35e7d90d21e9d5ae8551e3202e891701bc4a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 71.1 to 71.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 71.1 | 1 | 1 | [run](https://argusic.com/run/6ed82c8e-20ec-4c88-99c2-c3f462577500) |

## What was observed on a clean machine

Attempt 1:

- `CancelWorkflowAsyncOperationTest.cancelAsyncOperationAbandon fails in container , requires cloud Nexus provisioning`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
