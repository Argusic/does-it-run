# chidori

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ThousandBirdsInc/chidori, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/chidori

## Pinned environment

- Project commit: `223bb8779f63822c3e63a9a4347dda7483a02158`
- Test commit: `223bb8779f63822c3e63a9a4347dda7483a02158`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.1 to 16.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 8.1 | 0 | 0 | [run](https://argusic.com/run/31a8cefa-08dc-49f8-905f-ddce5d5e41c2) |
| 2 | pass | 100 | 9 | 16.7 | 2 | 2 | [run](https://argusic.com/run/8192196e-5482-4509-bf5e-945428f1ec2e) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `Rust toolchain not installed (no rustc/cargo)`
- 2 min: `1 flaky test failure out of 539: runtime::host_actor::tests::clean_restart_reaps_children_and_releases_their_names (assertion left=1 right=2, timing-dependent) , passes in isolation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
