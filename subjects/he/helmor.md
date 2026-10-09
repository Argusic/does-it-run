# helmor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dohooo/helmor, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/helmor

## Pinned environment

- Project commit: `a76cda1888265fb3e3208562d4b62616a4f0266a`
- Test commit: `a76cda1888265fb3e3208562d4b62616a4f0266a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.9 to 39.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 39 | 39.9 | 5 | 5 | [run](https://argusic.com/run/445a1bd9-5165-4acf-8691-c4ff34bf1a13) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `Rust binary linking failed: libgdk-3.so, libwebkit2gtk-4.1.so symlinks cannot be created in /usr/lib without root`
- 1 min: `scache wrapper configured in src-tauri/.cargo/config.toml but sccache not installed`
- 15 min: `Missing system dev packages for GTK/GLib/WebKit/JSCore/Clang/D-Bus pkg-config and headers`
- `Full frontend test suite (159 files) times out due to vitest transform latency`
- `Sidecar vendor build not supported on Linux`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
