# red

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/codersauce/red, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/red

## Pinned environment

- Project commit: `2ed85f3c4db4e3e2248e3b929f365cdade15a1dd`
- Test commit: `2ed85f3c4db4e3e2248e3b929f365cdade15a1dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29.9 to 29.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 29.9 | 4 | 4 | [run](https://argusic.com/run/36bc18d5-c868-4b8f-afbb-6bef5368a447) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `no Rust toolchain in container`
- 6 min: `red --check-config failed CFG303 on fresh HOME: default log_file cannot open because ~/.config/red not created on utility paths`
- 13 min: `cargo test --all-targets failed: editor::test::nonrecursive_directory_watch_snapshots_do_not_retain_directory_entries (overlayfs dir size 8192 and mtime can both be unchanged, so non-recursive snapshot missed new file)`
- 5 min: `cargo clippy --all-targets --all-features -- -D warnings failed with 46 pre-existing double_must_use errors at 6 async-trait/async-recursion sites on toolchain 1.99.1 (baseline before my changes also had 48 errors)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
