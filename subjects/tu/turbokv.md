# turbokv

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kingroryg/turbokv, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/turbokv

## Pinned environment

- Project commit: `5706b6ba02d86ff40d950276cfc4cf17bcd3a871`
- Test commit: `5706b6ba02d86ff40d950276cfc4cf17bcd3a871`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.6 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 4.6 | 1 | 1 | [run](https://argusic.com/run/fc0faf21-6186-427e-9f4f-38294cbd2ffa) |
| 2 | pass | 100 | 6 | 7.3 | 1 | 1 | [run](https://argusic.com/run/6dcf0e93-52dc-4b59-8371-4c020d760e3c) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `gxhash crate compile error: requires AES and SSE2 intrinsics but target-feature not enabled on x86_64`

Attempt 2:

- 1 min: `No Rust toolchain (rustc/cargo) present in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
