# macroquad

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/not-fl3/macroquad, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/macroquad

## Pinned environment

- Project commit: `8d602d3f8ebb8a3a582ee15d92983bbb81ee3ef6`
- Test commit: `8d602d3f8ebb8a3a582ee15d92983bbb81ee3ef6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.6 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 13.6 | 4 | 4 | [run](https://argusic.com/run/8ee7a351-9166-4602-bcdc-6ef119924355) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Rust toolchain not installed`
- 2 min: `cargo test --test coroutine_pause: 2 tests panicked with 'NATIVE_DISPLAY already set'`
- 5 min: `cargo test --test coroutine_pause: multi-test binary crashes with free(): invalid pointer when >1 X11-dependent test runs in same process`
- `cargo run --example window_conf fails: needs Wayland (XDG_RUNTIME_DIR not set)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
