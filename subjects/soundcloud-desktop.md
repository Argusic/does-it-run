# SoundCloud-Desktop

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zxcloli666/SoundCloud-Desktop, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/soundcloud-desktop

## Pinned environment

- Project commit: `50a71b2da5549510f2e7b6faa5acd4875010849e`
- Test commit: `50a71b2da5549510f2e7b6faa5acd4875010849e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 20.5 to 62.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.2 | 20.5 | 6 | 6 | [run](https://argusic.com/run/4f03833e-a4ca-48c9-b36a-0bb2eeab5aae) |
| 2 | fail | 50 | 62 | 62.6 | 9 | 9 | [run](https://argusic.com/run/e6743b8a-5861-483d-bcbd-1d9041f89ae2) |

## What was observed on a clean machine

Attempt 1:

- 0.4 min: `Node.js 18.19.1 too old for Vite 8 (requires 20.19+/22.12+)`
- 0.2 min: `pnpm not available in PATH`
- 0.2 min: `Rust toolchain not available`
- 0.1 min: `App/package.json requires private @sc/data and @sc/ui packages missing from registry`
- `desktop/src-tauri Rust build fails: system -dev packages missing (glib-2.0.pc, gobject-2.0.pc, webkit2gtk-4.1, libsoup-3.0) - cannot install without root`
- 0.1 min: `utils/call/client mock crate uses yanked wreq ^5`

Attempt 2:

- 5 min: `Node.js v18 installed, need v22+`
- 8 min: `No Rust toolchain installed`
- 3 min: `pnpm v9 installed, need v10+`
- 20 min: `Missing system -dev packages (glib, gtk3, webkit2gtk, etc.)`
- 4 min: `Missing libclang/LLVM for bindgen crate`
- 2 min: `Missing autoconf/automake/libtool for audiopus_sys build`
- 5 min: `Missing runtime .so files for webkit2gtk, libsoup, javascriptcoregtk`
- 10 min: `Missing transitive runtime libs (gstreamer, enchant, hyphen, manette, secret, wayland, etc.)`
- `WebKit subprocess paths hardcoded to /usr/lib/x86_64-linux-gnu/webkit2gtk-4.1/ without root access`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
