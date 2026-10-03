# Handy

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cjpais/Handy, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/handy

## Pinned environment

- Project commit: `8f9cf53cd1410cda26beea39ff802ac306e39585`
- Test commit: `8f9cf53cd1410cda26beea39ff802ac306e39585`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 19.2 to 66.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 19.2 | 0 | 0 | [run](https://argusic.com/run/5866dcaa-b7b3-4201-af9a-1c815f061cbe) |
| 2 | pass | 100 | 66 | 66.8 | 8 | 8 | [run](https://argusic.com/run/bda22dde-e8c1-40c6-b302-b95190ff1028) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `rustc not found (no Rust toolchain in container)`
- 3 min: `bun install script failed: unzip not installed and no root`
- 30 min: `cargo check failed: pkg-config glib-2.0 (and ~100 transitive dev packages) not installed`
- 12 min: `transcribe-cpp-sys CMake could not build Vulkan backend (Ubuntu glslc 2023.8 lacks GL_NV_cooperative_matrix2 support)`
- 8 min: `linker errors: non-PIC static archives (libX11.a, libdbus-1.a, etc) in extracted tree`
- 4 min: `runtime: libtranscribe.so.0.2 not found`
- 8 min: `runtime: WebKitNetworkProcess hardcoded to /usr/lib/x86_64-linux-gnu/webkit2gtk-4.1 (unwritable without root)`
- 1 min: `tauri dev/debug builds export bindings.ts relative to CWD; launching from repo root failed with PermissionDenied on /src/bindings.ts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
