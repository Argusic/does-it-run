# OpenLogi

**Verdict: runs.** Argusic Score 92.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AprilNEA/OpenLogi, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/openlogi

## Pinned environment

- Project commit: `7275072f58a18b81deef89b96c5a3d90cfd80dd4`
- Test commit: `7275072f58a18b81deef89b96c5a3d90cfd80dd4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 12.3 to 32.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 32.5 | 0 | 0 | [run](https://argusic.com/run/20c29462-cccd-46d5-ad1d-fd5dc3e59030) |
| 2 | pass | 93.33 | 18 | 12.3 | 3 | 2 | [run](https://argusic.com/run/46f778a7-badc-4034-b679-9edfc2f7f370) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Rust toolchain not installed`
- 5 min: `libclang not found by v4l2-sys-mit FFI bindgen`
- 3 min: `fontconfig.pc not found by yeslogic-fontconfig-sys (GPUI dependency)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
