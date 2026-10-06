# iwe

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iwe-org/iwe, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/iwe

## Pinned environment

- Project commit: `37a46877c0c8f10fdb25281c1ad687085c7b1b1f`
- Test commit: `37a46877c0c8f10fdb25281c1ad687085c7b1b1f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.4 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.4 | 1 | 1 | [run](https://argusic.com/run/c8ac1c7a-c3a9-45ec-b948-dcd6ac55c57d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `rustc/cargo not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
