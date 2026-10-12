# pup

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DataDog/pup, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/pup

## Pinned environment

- Project commit: `4493f8e0b6535f3599933df13673fb302a30bc5e`
- Test commit: `4493f8e0b6535f3599933df13673fb302a30bc5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 34.2 to 73.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 65 | 73.8 | 2 | 2 | [run](https://argusic.com/run/30e92f71-4433-47e6-944e-3980099cbced) |
| 2 | fail | 20 | n/a | 34.2 | 0 | 0 | [run](https://argusic.com/run/c6c6aef2-db19-4909-82ba-26a9bf18b944) |

## What was observed on a clean machine

Attempt 1:

- 55 min: `rustc SIGKILL (signal 9) compiling pinned dependency datadog-api-client at ~7.45GB RSS in all profiles (opt 0-3, -j 1, codegen-units 16-256, toolchains 1.89/1.95, native and wasm32-wasip1); cgroup memory.max is 8GB and the generated client`
- 10 min: `No pup binary could be built so no install target was produced and no test suite (cargo test) or CLI launch could run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
