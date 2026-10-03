# meetily

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Zackriya-Solutions/meetily, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/meetily

## Pinned environment

- Project commit: `0281737d87d26352fb0adc78c8c0975f691b23d1`
- Test commit: `0281737d87d26352fb0adc78c8c0975f691b23d1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 32.1 to 61.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.8 | 0 | 0 | [run](https://argusic.com/run/d8d2db61-1eb5-460b-b1d7-1dfe25e4d396) |
| 1 | pass with mocks | 92 | 58 | 61.1 | 6 | 6 | [run](https://argusic.com/run/d5e0ffd2-d66d-4d7c-bae5-2c5f1543e8fd) |
| 2 | fail | 50 | 28 | 32.1 | 2 | 2 | [run](https://argusic.com/run/b78dd06d-109f-4781-aa5b-e0be1cfd9c4e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing Rust toolchain (rustc, cargo)`
- 1 min: `Missing pnpm package manager`
- 32 min: `Missing system -dev packages for Tauri (glib, gtk, webkit2gtk, pcre2, freetype, harfbuzz, x11, mesa, dbus, atk, alsa, gstreamer, ayatana, dbusmenu, xslt, llvm/clang, libjpeg, libpng, tiff, webp, etc.)`
- 8 min: `Missing system runtime .so files for webkit2gtk, gstreamer, ayatana, dbusmenu, libxslt, etc.`
- 10 min: `WebKit subprocess path /usr/lib/... is hardcoded and cannot be written`
- 3 min: `Next.js frontend build ran out of memory (OOM killed)`

Attempt 2:

- `Missing system dev packages: libglib2.0-dev, webkit2gtk-4.1-dev, libgtk-3-dev, etc. cannot be installed without root`
- `Next.js production build OOM due to 1GB RAM limit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
