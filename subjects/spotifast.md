# spotifast

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crmne/spotifast, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/spotifast

## Pinned environment

- Project commit: `b5d579b857e61641c0933e64bb8e8d9e72506ae0`
- Test commit: `b5d579b857e61641c0933e64bb8e8d9e72506ae0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 54.1 to 87.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 48 | 54.1 | 4 | 4 | [run](https://argusic.com/run/5e6f10b0-4e60-4959-a749-0d76d6d882cf) |
| 2 | pass with mocks | 92 | 25 | 71.3 | 5 | 5 | [run](https://argusic.com/run/829cd607-671c-4886-9427-803d1a3f3968) |
| 3 | timeout | none | 78 | 87.5 | 5 | 5 | [run](https://argusic.com/run/f425fccc-bf54-43f0-9649-c14c0ada0fef) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Rust toolchain installed`
- 5 min: `Missing ALSA, PulseAudio, Wayland, XKB, and libffi development headers (no root access)`
- 2 min: `Linker (rust-lld) could not find -lasound, -lpulse, -lpulse-simple at link time`
- `projectm-sys (MilkDrop) build fails: X11/X.h not found`

Attempt 2:

- 1 min: `No Rust toolchain installed`
- 5 min: `Missing -dev packages (alsa, pulse, xkbcommon, wayland, libx11, libclang, etc.)`
- 2 min: `libclang not found at link time (libclang-18.so was a dead symlink without runtime library)`
- 1 min: `libGL and libgomp missing linker .so symlinks`
- 2 min: `Disk full during test (35GB target/)`

Attempt 3:

- 15 min: `Missing system -dev packages (alsa, pulse, dbus, x11, xcb, wayland, freetype, fontconfig, gl, egl, x11proto, libclang, libllvm)`
- 2 min: `Linker could not find -lasound, -lpulse, -lpulse-simple because .so symlinks from -dev packages pointed to .so.2.0.0 files not included in -dev`
- 3 min: `MilkDrop/projectM CMake build failed: X11/X.h not found`
- 3 min: `MilkDrop/bindgen: libclang not found`
- 2 min: `MilkDrop/bindgen: stdbool.h not found (missing clang resource dir)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
