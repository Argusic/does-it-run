# universal-game-mod-manager

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Indigo-0167/universal-game-mod-manager, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/universal-game-mod-manager

## Pinned environment

- Project commit: `ea301370dfaa3007665d5f32f344cd506ce4fa7c`
- Test commit: `ea301370dfaa3007665d5f32f344cd506ce4fa7c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 10.6 to 13.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 18 | 10.6 | 4 | 4 | [run](https://argusic.com/run/e1d0ea24-7411-4233-b413-4d063c424da2) |
| 2 | pass | 100 | 12 | 13.1 | 4 | 4 | [run](https://argusic.com/run/64e9e92d-600e-4c5e-83cb-805fa4b73aac) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Rust toolchain not installed`
- 2 min: `Package fontconfig.pc not found , yeslogic-fontconfig-sys build.rs needs pkg-config to find fontconfig`
- 2 min: `Crate names mismatch , Cargo.toml uses universal-game-mod-manager-backend and universal-game-mod-manager-proc-macros, but source code imports rai_pal_backend and rai_pal_proc_macros`
- 1 min: `Linker -lfontconfig not found at build time , dev package not installed so libfontconfig.so symlink is missing`

Attempt 2:

- 1 min: `Missing Rust toolchain (rustc 1.100.0 was installed via rustup)`
- 8 min: `Missing C dev headers/libs (fontconfig, freetype, X11, xcb, xkbcommon, wayland, EGL, dbus) - no pkg-config .pc files`
- 1 min: `Crate name mismatch: source uses 'rai_pal_proc_macros' and 'rai_pal_backend' but package names are 'universal-game-mod-manager-*'`
- 1 min: `Linker could not find -lfontconfig -lfreetype because .so symlinks pointed to missing .so.1 files in the sysroot`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
