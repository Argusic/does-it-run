# browser-control

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/keon/browser-control, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/browser-control

## Pinned environment

- Project commit: `b352a1ac017113b25c82fac8b78ddedd597ddb74`
- Test commit: `b352a1ac017113b25c82fac8b78ddedd597ddb74`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.6 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 9.6 | 4 | 4 | [run](https://argusic.com/run/cd162a20-7cdb-4393-9aa2-f20280bf65d0) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Rust toolchain (rustup/cargo/rustc) installed in container`
- 3 min: `No Chrome/Chromium browser available on system`
- 1 min: `Chrome crashes without --no-sandbox flag in this container environment (no FUSE/kernel sandbox support)`
- 0.5 min: `cargo fmt --check flagged formatting issues in src/cloud.rs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
