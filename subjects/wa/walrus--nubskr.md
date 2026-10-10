# walrus

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nubskr/walrus, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/f0b94ddf-6ea0-454e-bbb9-4d84eedaaa57

## Pinned environment

- Project commit: `89a38a0b6dd058644f8e4eac4ac1c179bf45ece7`
- Test commit: `89a38a0b6dd058644f8e4eac4ac1c179bf45ece7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 64 to 64 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 30 | 64 | 5 | 4 | [run](https://argusic.com/run/f0b94ddf-6ea0-454e-bbb9-4d84eedaaa57) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `clang-sys build failed: missing libclang.so for rocksdb bindgen`
- 3 min: `librocksdb-sys build failed: stdbool.h not found by clang`
- 1 min: `librocksdb-sys build failed: cannot load libclang-20.so.20 shared library`
- `test_env_var_race_condition test panics reproducing a known env-var race`
- 2 min: `0.0.0.0 raft-host address causes unreachable peers in Raft replication`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
