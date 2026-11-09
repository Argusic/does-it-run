# Codex-X

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yynxxxxx/Codex-X, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/codex-x

## Pinned environment

- Project commit: `8f018fddd3ee1a68464e4df8765eb370ede0c76f`
- Test commit: `8f018fddd3ee1a68464e4df8765eb370ede0c76f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 6 to 40 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 6 | 5 | 5 | [run](https://argusic.com/run/c07fe855-75a5-4172-ba3c-afaef3661a3d) |
| 2 | pass | 100 | 40 | 40 | 9 | 9 | [run](https://argusic.com/run/849db2b4-75a7-42c1-bb63-4d977abef151) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed`
- 2 min: `Rust/Cargo not installed`
- 2 min: `Node.js 18 too old for Vite 7 build (crypto.hash not a function)`
- 1 min: `Tests import .ts files which Node.js 18 can't load natively`
- `Tauri Rust backend build fails , missing system libraries glib-2.0.pc, gtk-3, webkit2gtk, etc.`

Attempt 2:

- 1 min: `pnpm not found in PATH`
- 3 min: `Node.js v18.19.1 too old for Vite 7 (requires 20.19+)`
- `Vite 7: crypto.hash is not a function on Node 18`
- 5 min: `Rust build: pkg-config could not find glib-2.0, gio-2.0, gtk+-3.0, webkit2gtk-4.1, libsoup-3.0, etc.`
- 5 min: `Rust build: rust-lld unable to find libraries (lgdk-3, lz, lwebkit2gtk-4.1, etc.)`
- 3 min: `Runtime: undefined symbol gst_context_set_gl_display from stub libgstgl`
- 2 min: `Runtime: libdw.so.1 and liborc-0.4.so.0 not found`
- 1 min: `Runtime: libxslt.so.1 not found`
- `Desktop app: WebKitNetworkProcess not found at hardcoded /usr/lib/x86_64-linux-gnu/webkit2gtk-4.1/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
