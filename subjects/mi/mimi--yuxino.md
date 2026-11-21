# mimi

**Verdict: runs with mocks.** Argusic Score 89.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yuxino/mimi, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/c9f8c2e6-78e0-4014-ad11-0611c30837db

## Pinned environment

- Project commit: `9eae2b87be8092a92dc5bca98b793d1e36917b10`
- Test commit: `9eae2b87be8092a92dc5bca98b793d1e36917b10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 21.1 to 36.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 21 | 21.1 | 4 | 3 | [run](https://argusic.com/run/c9f8c2e6-78e0-4014-ad11-0611c30837db) |
| 2 | pass with mocks | 92 | 36 | 36.4 | 7 | 7 | [run](https://argusic.com/run/9bf82f7f-b73f-444e-8c58-c4f1030ed8cd) |

## What was observed on a clean machine

Attempt 1:

- `Node.js v18 installed (needs ^20.19.0) - engine check warned but all commands succeeded`
- 1 min: `Rust toolchain not installed`
- 15 min: `Missing system -dev libraries (no root) - webkit2gtk, GTK3, GLib, libsoup, X11 protos`
- 3 min: `Linker failed to find system .so files at link time`

Attempt 2:

- 2 min: `Rust not installed`
- 3 min: `Node.js v18 too old (requires 20+)`
- 8 min: `Missing Tauri/WebKit system -dev libraries (libwebkit2gtk-4.1-dev, libgtk-3-dev, etc.)`
- 4 min: `gio-2.0.pc had unsatisfed transitive pkg-config deps (zlib, mount, libselinux, freetype2, fontconfig, x11, etc.)`
- 3 min: `Rust lld linker could not find extracted .so libraries`
- 5 min: `WebKit helper binaries hardcode /usr/lib/... path (not writable)`
- 5 min: `Missing appindicator/dbusmenu/dbus runtime libraries for tray icon`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
