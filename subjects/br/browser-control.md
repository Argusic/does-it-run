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
- Valid runs: 2; wall time 9.6 to 15.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 9.6 | 4 | 4 | [run](https://argusic.com/run/cd162a20-7cdb-4393-9aa2-f20280bf65d0) |
| 2 | pass | 100 | 12 | 15.2 | 5 | 5 | [run](https://argusic.com/run/043e2721-7034-4e3c-93c2-651e9b6906a7) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Rust toolchain (rustup/cargo/rustc) installed in container`
- 3 min: `No Chrome/Chromium browser available on system`
- 1 min: `Chrome crashes without --no-sandbox flag in this container environment (no FUSE/kernel sandbox support)`
- 0.5 min: `cargo fmt --check flagged formatting issues in src/cloud.rs`

Attempt 2:

- 2 min: `No Rust toolchain installed`
- 1 min: `No Chrome/Chromium available`
- 1 min: `Chrome crashes with sandbox error (--no-sandbox needed)`
- 1 min: `Chrome 119+ HTTP CDP discovery fails without --remote-allow-origins=*`
- 1 min: `Formatting check failed in verify.sh`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
