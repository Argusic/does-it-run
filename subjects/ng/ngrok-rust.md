# ngrok-rust

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ngrok/ngrok-rust, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/ngrok-rust

## Pinned environment

- Project commit: `e8664d8877eb50cb909f3c2f62b5f0c50312a35f`
- Test commit: `e8664d8877eb50cb909f3c2f62b5f0c50312a35f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14.9 to 14.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 14 | 14.9 | 2 | 1 | [run](https://argusic.com/run/c6d58f58-2df5-4e00-8207-a32e37cb0d49) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Rust toolchain present in container (cargo/rustc not found); flake.nix devShell unusable because nix is not installed.`
- 2 min: `'cargo test --workspace' failed: doctest ngrok/src/../README.md line 83 exits 1 with ERR_NGROK_4018 'session is not authenticated'.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
