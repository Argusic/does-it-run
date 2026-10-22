# crabtalk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crabtalk/crabtalk, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/crabtalk

## Pinned environment

- Project commit: `93f2f024acabe36cc9b373d6d4a187c1047952c6`
- Test commit: `93f2f024acabe36cc9b373d6d4a187c1047952c6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.6 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 9.6 | 2 | 2 | [run](https://argusic.com/run/6265cece-b952-44c1-bec3-ff27c4511650) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `cargo: not found in PATH , Rust toolchain not installed`
- 0.5 min: `protoc not found , prost-build requires the protobuf compiler`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
