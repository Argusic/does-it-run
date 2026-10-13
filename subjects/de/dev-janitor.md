# Dev-Janitor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cocojojo5213/Dev-Janitor, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/dev-janitor

## Pinned environment

- Project commit: `e06fd6ee7838e80edf1ffcb3f6b67238732f8a16`
- Test commit: `e06fd6ee7838e80edf1ffcb3f6b67238732f8a16`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 3.2 | 1 | 1 | [run](https://argusic.com/run/422b3003-62a4-4fc6-8f3c-0dabe97f5710) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Desktop-feature Rust builds (cargo check / cargo test / tauri build) fail: glib-sys, gio-sys, webkit2gtk-sys system dev packages (glib-2.0.pc, gio-2.0.pc, webkit2gtk-4.1, etc.) are not installed and apt-get is unavailable (no root; plain 'r`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
