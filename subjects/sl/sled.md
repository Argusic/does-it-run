# sled

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spacejam/sled, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/sled

## Pinned environment

- Project commit: `e449d17111f4a097e1c66b6db241962ccb6a4136`
- Test commit: `e449d17111f4a097e1c66b6db241962ccb6a4136`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.3 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.18 | 16.3 | 2 | 2 | [run](https://argusic.com/run/6b1f3396-f3ba-44bc-9ce8-9e1bf7ad0ace) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `tree_bug_10, tree_bug_43, tree_bug_46 fail with WouldBlock (EAGAIN) on try_lock_exclusive() in heap recovery when tests run in parallel`
- 0.1 min: `test_tree_failpoints skipped: feature 'failpoints' not defined in Cargo.toml`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
