# opsli-boot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hiparker/opsli-boot, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/opsli-boot

## Pinned environment

- Project commit: `80becfa375db9e929243e27ee2e32620f5dae8ab`
- Test commit: `80becfa375db9e929243e27ee2e32620f5dae8ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.6 to 18.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 18.6 | 5 | 5 | [run](https://argusic.com/run/406270a6-cf5e-4a6d-b078-6490cb207929) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `JDK 22 and Maven 3.9.6 not pre-installed`
- 1 min: `Test JUnit 4 import not compatible with JUnit 5 Platform runner (no vintage engine)`
- 1 min: `Placeholder resolution error for springdoc.swagger-ui.enabled in local profile`
- 3 min: `MySQL 8.0 missing shared libraries (libevent, libaio, libprotobuf)`
- 2 min: `Redis 7.0 missing shared libraries (liblzf, libjemalloc)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
