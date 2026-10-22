# hummingbird

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hummingbird-player/hummingbird, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/hummingbird

## Pinned environment

- Project commit: `15835949458d3750c2f85c1178263edad0a476a8`
- Test commit: `15835949458d3750c2f85c1178263edad0a476a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 36.9 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/3f4aa884-040e-46fa-9f3c-29a679510f78) |
| 2 | pass | 100 | 30 | 36.9 | 5 | 5 | [run](https://argusic.com/run/a185ccb0-41de-4fa0-b55d-12bc6dd502cf) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `No Rust toolchain installed in container`
- 5 min: `Missing -dev packages for Linux system libraries (alsa, xkbcommon, x11, pulse, fontconfig, pipewire, dbus, wayland, xcb, zlib, png, brotli, expat)`
- 5 min: `Missing libclang for bindgen crate (libpipewire/spa FFI generation)`
- 1 min: `Missing lld-18 linker used by cargo`
- 2 min: `Linker could not find native .so files (broken symlinks in dev packages)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
