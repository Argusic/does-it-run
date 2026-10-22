# sqz

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ojuschugh1/sqz, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/sqz

## Pinned environment

- Project commit: `ff33708e2a311e514e3d73a5bd04c021d4fd4527`
- Test commit: `ff33708e2a311e514e3d73a5bd04c021d4fd4527`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.1 to 13.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 13.1 | 2 | 2 | [run](https://argusic.com/run/6503e567-081b-4f4c-b4f3-b523f0c5d00a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `global npm install failed: EACCES mkdir /usr/local/lib/node_modules/sqz-cli (no root)`
- 2 min: `no Rust toolchain in container (cargo/rustc not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
