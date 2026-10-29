# screencapturekit-rs

**Verdict: could not verify.** Argusic Score 10 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/doom-fish/screencapturekit-rs, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/screencapturekit-rs

## Pinned environment

- Project commit: `a46de0a44d67622a0e82de0bae4e02a314c7b727`
- Test commit: `a46de0a44d67622a0e82de0bae4e02a314c7b727`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.9 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 4 | 8.2 | 4 | 0 | [run](https://argusic.com/run/b127fea2-8a9f-42ca-9bf2-579914025d3d) |
| 2 | fail | 20 | 25 | 5.9 | 3 | 3 | [run](https://argusic.com/run/797d7e6c-55a7-4fe3-96e7-0affcd162b3d) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `**Environmental blocker**: repository is macOS-only. README and CI require macOS 13.0+ SDK, Xcode Command Line Tools, and the Apple 'swift' toolchain; CI only runs on macos-26. The host is Ubuntu 24.04 x86_64 without 'swift'/'xcrun'/'xcodeb`
- `**The only documented non-Apple build path (docs.rs mode, 'DOCS_RS=1') does not compile on native Linux**: 'apple-cf v0.11.7' uses '#[link(name=..., kind="framework")]' which rustc rejects on Linux targets (E0455: link kind 'framework' is o`
- `Running the test suite is impossible: 'cargo test --target x86_64-apple-darwin' (the only target where compilation gets past the framework-link errors) cannot link on Linux , dev-dependency C build (blake3 via eframe/bevy/wgpu grahics stack`
- `**Maximum achievable verification reached**: with the crate's own source typechecked for the Apple target in the documented docs.rs mode: 'DOCS_RS=1 cargo check --target x86_64-apple-darwin --all-features' -> exit 0, 'Finished dev profile'`

Attempt 2:

- 12 min: `cargo build fails: apple-metal v0.10.4 build script panics 'Failed to build Swift bridge: No such file or directory' because no Swift/Xcode toolchain exists in this Linux container`
- 8 min: `DOCS_RS=1 (the build.rs escape hatch) still fails on Linux: rustc E0455 'link kind framework is only supported on Apple targets' in apple-cf v0.11.7 (6 sites: cg/affine.rs:108, cg/display.rs:7, cg/display.rs:24, cg/mod.rs:21, cv/buffer.rs:2`
- 5 min: `cargo test (clean checkout) fails in apple-metal-0.10.4/build.rs:49:39 'Failed to build Swift bridge: No such file or directory'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
