# seekdb

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oceanbase/seekdb, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/seekdb

## Pinned environment

- Project commit: `ab26e64cfbb81ac16f5ca95a475657f44a14f3b3`
- Test commit: `ab26e64cfbb81ac16f5ca95a475657f44a14f3b3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 37.2 to 64.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 37.2 | 0 | 0 | [run](https://argusic.com/run/1fa674a2-b46b-4171-81ae-a1c8e6db2f1b) |
| 2 | fail | 20 | 65 | 64.9 | 6 | 6 | [run](https://argusic.com/run/e10e7b9d-e5c3-4d02-8a17-50bd567552a0) |

## What was observed on a clean machine

Attempt 2:

- 10 min: `dep_create.sh requires wget which is not installed`
- 15 min: `dep_create.sh requires rpm2cpio and cpio which are not installed`
- 2 min: `Python pip install pyseekdb blocked by externally-managed-environment`
- 5 min: `Rust toolchain not active`
- 10 min: `C++ build blocked: bison requires m4 which is not installed in the container`
- 30 min: `OceanBase dependency mirror very slow (~40KB/s for large RPMs)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
