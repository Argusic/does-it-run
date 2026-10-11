# mongo-cxx-driver

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mongodb/mongo-cxx-driver, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/mongo-cxx-driver

## Pinned environment

- Project commit: `87b0d6830003195a7cb527534d6be5e6dda9952a`
- Test commit: `87b0d6830003195a7cb527534d6be5e6dda9952a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.1 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 16.1 | 1 | 1 | [run](https://argusic.com/run/3d598788-817f-4c31-b4ae-ca7ed466e1d7) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `3 CTest targets failed with 'no such command: configureFailPoint' (CommandNotFound) because mongod lacked --setParameter enableTestCommands=1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
