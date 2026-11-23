# codeseek

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CodeBendKit/codeseek, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/codeseek

## Pinned environment

- Project commit: `981bd23800d1ba6bd0b26c70942e5d0392c6c8b1`
- Test commit: `981bd23800d1ba6bd0b26c70942e5d0392c6c8b1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.9 to 15.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 14.9 | 2 | 2 | [run](https://argusic.com/run/7e13045b-fac5-4f3d-950e-026d0be7db6d) |
| 2 | pass | 100 | 38 | 15.5 | 4 | 4 | [run](https://argusic.com/run/20511446-0e4d-4ab5-886e-2701ec08ff8d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Rust toolchain in container`
- 2 min: `lance-encoding requires protoc for protobuf codegen`

Attempt 2:

- 2 min: `rustc not available in container`
- 2 min: `protoc not available, required by lance-encoding build dependency`
- 1 min: `protoc could not find google/protobuf/empty.proto include`
- 1 min: `Node v18.19.1 < required >=20.0.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
