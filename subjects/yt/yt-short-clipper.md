# yt-short-clipper

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jipraks/yt-short-clipper, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/yt-short-clipper

## Pinned environment

- Project commit: `f6d6d98f3bcee1b056cd49990a7f7176c55ac10b`
- Test commit: `f6d6d98f3bcee1b056cd49990a7f7176c55ac10b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 24.8 to 25.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 24.8 | 0 | 0 | [run](https://argusic.com/run/a7ad21a6-15a9-4a3a-9642-a9758b07d89d) |
| 2 | pass with mocks | 92 | 25 | 25.5 | 9 | 9 | [run](https://argusic.com/run/0fbd3333-1585-4633-bc2c-216cf63a6599) |

## What was observed on a clean machine

Attempt 2:

- `npm install succeeded with EBADENGINE warnings for Node v18 vs required v20`
- 1 min: `@tailwindcss/oxide native binding missing for Linux x64`
- 1 min: `pip install blocked by externally-managed-environment (PEP 668)`
- 12 min: `Rust toolchain not installed`
- 10 min: `System dev libraries (glib-2.0, webkit2gtk-4.1, gtk-3, soup-3.0, javascriptcoregtk, etc.) missing; no root access to apt install`
- 5 min: `Rust compilation failed: resource path binaries/ytclip-sidecar-x86_64-unknown-linux-gnu missing`
- 1 min: `Rust linker failed: missing -ldbus-1, -lgobject-2.0, -lwebkit2gtk-4.1, etc.`
- 1 min: `WebKitNetworkProcess not found at hardcoded /usr/lib/... path (no root)`
- `libwebkit2gtkinjectedbundle.so not found at new path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
