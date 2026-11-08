# sandstorm

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deeplethe/sandstorm, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/sandstorm

## Pinned environment

- Project commit: `d27ab7c452126e3b34987b84d3c72cb41fc3fd16`
- Test commit: `d27ab7c452126e3b34987b84d3c72cb41fc3fd16`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 11.4 to 11.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 11.6 | 3 | 3 | [run](https://argusic.com/run/f3a4b2b6-ca08-49f6-9948-e835f1461b9c) |
| 2 | pass | 100 | 28 | 11.4 | 4 | 4 | [run](https://argusic.com/run/1e20d91c-f3f6-4fdd-9170-3cdcc599cb8c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `zstd not installed: 3 tests failed (crates/sandstorm-core/src/node/detach_tests.rs)`
- 1 min: `/run/sandstorm/ not writable: node mode failed to create /run/sandstorm/gateway-ports and /run/sandstorm/veth`
- 3 min: `iptables and ip not found: node backend failed with 'No such file or directory'`

Attempt 2:

- 3 min: `container had no Rust toolchain (cargo/rustc missing)`
- 2 min: `container had Node 18 but the project needs Node >=20/22 (README says 22.12+)`
- 5 min: `3 cargo unit tests failed: 'starting zstd to archive layer: No such file or directory' (detach_tests)`
- 4 min: `serve --master --node refuses with 'creating /run/sandstorm/gateway-ports: Permission denied' (hard-coded root-only path)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
