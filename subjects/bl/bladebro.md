# bladebro

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dondai44423/bladebro, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/bladebro

## Pinned environment

- Project commit: `0300ee0e3095fed5709f0721d7b1caf323764d5c`
- Test commit: `0300ee0e3095fed5709f0721d7b1caf323764d5c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.1 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 8.1 | 5 | 5 | [run](https://argusic.com/run/df9fcfe9-97bf-4b6e-9ce7-86e28ef1e613) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npm install -g EACCES: /usr/local/lib/node_modules/bladebro`
- 1.5 min: `No Rust toolchain installed`
- 1 min: `Chrome/Chromium not found on system`
- 0.5 min: `cargo clippy reported 6 eprintln!["..."] with nonstandard-macro-braces (Rust 1.99)`
- 0.1 min: `Chrome for Testing crashes with SIGTRAP (crashpad handler missing execute bit)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
