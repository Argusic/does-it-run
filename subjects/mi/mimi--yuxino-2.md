# Mimi

**Verdict: runs with mocks.** Argusic Score 66.4 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yuxino/Mimi, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/2c2a0102-20d8-40a6-9f5e-e7badbd6169d

## Pinned environment

- Project commit: `a0ac37f4adcc52af910767a299a2b7dbf67819da`
- Test commit: `a0ac37f4adcc52af910767a299a2b7dbf67819da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 9.4 to 35.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 43.33 | 12 | 9.4 | 3 | 2 | [run](https://argusic.com/run/2c2a0102-20d8-40a6-9f5e-e7badbd6169d) |
| 2 | pass with mocks | 89.5 | 36 | 35.9 | 8 | 7 | [run](https://argusic.com/run/619ddf4c-1b29-44ac-9602-928c7a74bc08) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18 is too old; project requires ^20.19.0`
- 1 min: `Rust toolchain not installed`
- `System libraries missing: glib-2.0, webkit2gtk-4.1, libsoup-3.0, gtk+-3.0, libpulse, and their -dev packages`

Attempt 2:

- 6 min: `No Rust toolchain (rustc/cargo) and Node 18 below the required 20.19+ were installed in the bare container`
- 12 min: `No WebKitGTK/GTK/libsoup/ayatana dev libraries and pkg-config files were present; apt-get install requires root`
- 3 min: `aec-rs-sys build script failed: bindgen could not find libclang`
- 7 min: `Linker could not find -lgtk-3 etc: dev symlinks were dangling because runtime library debs were not extracted`
- 2 min: `App aborted at startup: 'development builds require the isolated Tauri identifier'`
- 6 min: `WebKit hardcodes /usr/lib/x86_64-linux-gnu/webkit2gtk-4.1 for its helper processes, which is unwritable without root, so WebKitNetworkProcess failed to spawn`
- 2 min: `Nonfatal WebKit GSettings ERROR 'Settings schema org.gnome.system.proxy is not installed'`
- `Live provider verification needs real third-party credentials; UI-test mode stubs the session per repo design`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
