# OpenWiki

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kdsz001/OpenWiki, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/7b74e858-53ae-432e-a844-91bec34f5e0e

## Pinned environment

- Project commit: `0e675dd2aa482a76993ab51cc2e4a0ae59044434`
- Test commit: `0e675dd2aa482a76993ab51cc2e4a0ae59044434`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 33.2 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/7b74e858-53ae-432e-a844-91bec34f5e0e) |
| 2 | fail | 80 | 33 | 33.2 | 7 | 7 | [run](https://argusic.com/run/93d3444d-1555-4062-adac-7ac196f2c450) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Rust toolchain not pre-installed`
- 3 min: `Missing pkg-config .pc files for glib, gobject, gtk, webkit, soup, javascriptcore, cairo, pango, harfbuzz, pcre2, x11, xcb, and ~50 more - Rust crate build scripts (glib-sys, gobject-sys, gtk-sys, tauri) use pkg-config for C library detecti`
- 5 min: `Missing runtime .so files for libwebkit2gtk-4.1, libjavascriptcoregtk-4.1, libsoup-3.0, gstreamer, xslt, harfbuzz-icu, enchant, hyphen, secret, manette, wayland-server, orc, libdw`
- 1 min: `'macos-private-api' Tauri feature not in allowlist on Linux`
- 3 min: `WebKitGTK library hardcodes /usr/lib/x86_64-linux-gnu/webkit2gtk-4.1/ path for subprocesses (WebKitNetworkProcess, WebKitWebProcess, MiniBrowser)`
- 3 min: `libappindicator-sys panics on missing tray icon shared libraries (ayatana-appindicator3 -> dbusmenu-gtk3 -> ayatana-ido3 -> ayatana-indicator3)`
- 2 min: `Linker cannot find .so files from symlinks in /home/runner/.local/lib`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
