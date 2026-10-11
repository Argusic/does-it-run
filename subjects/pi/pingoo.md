# pingoo

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pingooio/pingoo, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/pingoo

## Pinned environment

- Project commit: `f388e34e7adb4be3e1cf5629a07a009b228929bb`
- Test commit: `f388e34e7adb4be3e1cf5629a07a009b228929bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 10.6 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 10.6 | 3 | 3 | [run](https://argusic.com/run/9c0ecc7d-b026-4dc0-b1bc-33ce29ba5377) |
| 2 | pass | 100 | 15 | 16.1 | 3 | 3 | [run](https://argusic.com/run/bab23741-e75a-4cb9-aeb7-eaac711a1d99) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain (rustc, cargo) not installed`
- `captcha/dist directory missing`
- 7 min: `Config path hardcoded to /etc/pingoo/pingoo.yml (root-only)`

Attempt 2:

- 3 min: `captcha dist folder missing - npm build required before Rust compile`
- 10 min: `hardcoded /etc/pingoo paths unwritable (no root)`
- `info log message still prints DEFAULT_CONFIG_FILE constant instead of resolved path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
