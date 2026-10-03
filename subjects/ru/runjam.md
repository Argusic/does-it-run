# runjam

**Verdict: runs.** Argusic Score 85 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/peintune/runjam, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/runjam

## Pinned environment

- Project commit: `5f8e67ac2185bde763e40f7b4538e4d13b591912`
- Test commit: `5f8e67ac2185bde763e40f7b4538e4d13b591912`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 9.1 to 16 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 16 | 3 | 3 | [run](https://argusic.com/run/5904b4b7-dc72-42de-9439-5f976ed2bb58) |
| 2 | fail | 70 | 8 | 9.1 | 2 | 1 | [run](https://argusic.com/run/b1dbe870-b512-477f-aa52-0650d578cb65) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `@tailwindcss/oxide missing native binding for linux-x64-gnu`
- 1 min: `cargo not found (no Rust toolchain)`
- 8 min: `Tauri Linux system -dev packages missing (glib-2.0, gtk3, pango, cairo, webkit2gtk-4.1, javascriptcoregtk-4.1, libsoup-3.0)`

Attempt 2:

- 2 min: `TailwindCSS native binding not installed due to Node 18 engine mismatch`
- 22 min: `Rust/Tauri backend cannot compile: missing system libraries (libwebkit2gtk-4.1-dev, libgobject-2.0-dev, libsoup-3.0-dev). No root to install them.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
