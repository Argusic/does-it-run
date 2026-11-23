# RustWTM

**Verdict: could not verify.** Argusic Score 40 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RustWTM/RustWTM, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/rustwtm

## Pinned environment

- Project commit: `1f396ec3785dde57c431ae3011e36c5f8becc5c0`
- Test commit: `1f396ec3785dde57c431ae3011e36c5f8becc5c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.3 to 45.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 44.7 | 45.2 | 6 | 6 | [run](https://argusic.com/run/a2cabcab-ec05-40d6-9592-4ecdae3e0748) |
| 2 | fail | 0 | 8 | 5.3 | 2 | 0 | [run](https://argusic.com/run/55164567-d07f-4e73-a6c8-2af3eb58251e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed in container`
- 1 min: `windows-future crate fails on Linux host (cfg(windows)-gated function 'submit')`
- 1 min: `Missing glib-2.0 and other GTK development libraries for native Linux build`
- 10 min: `build.rs resource embedding fails due to missing windres and mingw toolchain`
- 3 min: `libsqlite3-sys C compilation fails: #include_next <stdarg.h> cannot find platform header`
- 5 min: `Linking fails: crt2.o and Windows import libraries not found by mingw ld`

Attempt 2:

- `RustWTM is a Windows-only project. Crate wtm-sys has #![cfg(windows)], depends on the windows crate (Win32/NT APIs), and uses winreg (Windows Registry). All other crates transitively depend on wtm-sys or winreg, making the workspace unbuild`
- `System library headers (libglib2.0-dev, libgtk-3-dev, etc.) required by eframe/GTK3 accessibility dependencies (glib-sys, gobject-sys) cannot be installed , no root access.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
