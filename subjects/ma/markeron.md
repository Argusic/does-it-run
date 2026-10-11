# markeron

**Verdict: could not verify.** Argusic Score 36.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ifer47/markeron, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/markeron

## Pinned environment

- Project commit: `3e87b1cc2980776c49b691a573d5e9b04b04e9d6`
- Test commit: `3e87b1cc2980776c49b691a573d5e9b04b04e9d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 5 | 6 | 1 | 0 | [run](https://argusic.com/run/2e9bce22-9cf8-49c0-a74d-1d546ba50305) |
| 2 | fail | 43.33 | 24 | 20.2 | 3 | 2 | [run](https://argusic.com/run/3f5fa18d-ddb3-49bd-8b33-8f19fd45e134) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Rust/Tauri build cannot compile on Linux , system GTK/WebKit dev libraries (glib-2.0-dev, libwebkitgtk-6.0-4-dev, etc.) are missing and cannot be installed without root. The project explicitly supports only Windows and macOS per CONTRIBUTIN`

Attempt 2:

- 2 min: `Node.js v18.19.1 in container instead of required v24.15.0`
- 20 min: `Missing GTK3/GLib/WebKit system dev libraries for Tauri Rust build`
- `Rust/Tauri cargo check fails on Linux by design - compile_error! guard at src/lib.rs:2`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
