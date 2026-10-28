# geo-downloader

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gaopengbin/geo-downloader, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/geo-downloader

## Pinned environment

- Project commit: `0496e0cb8496b060f2a25720b338b56845abb9ec`
- Test commit: `0496e0cb8496b060f2a25720b338b56845abb9ec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 24.4 to 49.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 20 | 24.4 | 4 | 4 | [run](https://argusic.com/run/ea26a273-0ef7-4c34-9865-913ec5a832e7) |
| 2 | pass | 100 | 47 | 49.6 | 5 | 5 | [run](https://argusic.com/run/e5d1abef-f103-42e8-a938-e382ceb19236) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Missing system -dev packages for Tauri (webkit2gtk-4.1, glib, gtk3, cairo, pango, libsoup3, etc.)`
- 2 min: `Node.js 18 too old for Vite 8`
- 1 min: `Missing @rolldown/binding-linux-x64-gnu native module`
- `Tauri desktop app cannot launch in container: missing webkit2gtk runtime (libgstreamer, libsecret, libmanette, etc.) not satisfiable without root`

Attempt 2:

- 2 min: `Node.js v18 too old (requires 20+)`
- 30 min: `Missing -dev packages for Tauri (libwebkit2gtk-4.1-dev, libglib2.0-dev, etc.) - no sudo access`
- 2 min: `Static .a libs in sysroot conflicted with dynamic linking (dbus-1 needed libsystemd)`
- 3 min: `rust-lld could not find system libraries`
- 5 min: `Missing runtime .so files (libdw, liborc, libzstd, libelf, etc.) needed by WebKit/gstreamer`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
