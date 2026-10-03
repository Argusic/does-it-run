# onedev

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/theonedev/onedev, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/onedev

## Pinned environment

- Project commit: `d44925c47c37992c828ea673a5f9620539bc3ff2`
- Test commit: `d44925c47c37992c828ea673a5f9620539bc3ff2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 23.9 to 38.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 4.5 | 26.7 | 1 | 1 | [run](https://argusic.com/run/7ba5a63e-aff6-4b40-80c8-d7b0b955c262) |
| 2 | fail | 20 | n/a | 23.9 | 0 | 0 | [run](https://argusic.com/run/a26dd40a-1eef-44c3-b7e5-0faf689c76d5) |
| 3 | pass | 100 | 38 | 38.2 | 11 | 11 | [run](https://argusic.com/run/55094d67-0645-48a8-bebf-bbd2a6bef4e2) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `Byte Buddy 1.12.14 does not support Java 21 (65) - requires net.bytebuddy.experimental VM property`

Attempt 3:

- 2 min: `Java not found on system`
- 1 min: `Maven not found on system`
- 10 min: `server-ee submodule requires authentication (private repo)`
- `server-product build fails on server-ee dependency`
- 1 min: `Sandbox lib JARs conflict with target/classes causing 'More than one version' error`
- 5 min: `Missing Guice bindings for ClusterService, AuditService, JobTerminalService, StorageService, SubscriptionService`
- 2 min: `Hazelcast NPE in DefaultClusterService`
- 2 min: `initWithLead skipped, no DB schema created`
- 3 min: `runOnAllServers returned empty map, settings cache not populated`
- 1 min: `Map.of() rejects null values from task.call()`
- 1 min: `Stale HSQLDB causing 'object not found' SQL errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
