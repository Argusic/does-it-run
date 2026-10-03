# trippy

**Verdict: runs.** Argusic Score 70.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fujiapple852/trippy, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/trippy

## Pinned environment

- Project commit: `2e69fcfee7126c1f8449d8b907c21b07d68fad25`
- Test commit: `2e69fcfee7126c1f8449d8b907c21b07d68fad25`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services, no run possible
- Valid runs: 3; wall time 5.9 to 33.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 33.1 | 2 | 2 | [run](https://argusic.com/run/11be9f23-5c3b-41cf-a348-2a4379523b85) |
| 2 | pass with mocks | 92 | 2 | 5.9 | 0 | 0 | [run](https://argusic.com/run/df5b9cd5-1315-41eb-bf6d-f0fd6d5532df) |
| 3 | fail | 20 | n/a | 9.6 | 0 | 0 | [run](https://argusic.com/run/d1d34257-d1e6-4a89-859d-cd0e2960e404) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Rust toolchain not installed (rustup, rustc, cargo missing)`
- 9.5 min: `No C compiler (cc/gcc) available on the system, needed by Rust's cc crate for build scripts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
