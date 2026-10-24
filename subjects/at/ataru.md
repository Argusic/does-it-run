# Ataru

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lovstudio/Ataru, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/ataru

## Pinned environment

- Project commit: `44ad0d435d501efc2b937b6083e04f3551884c33`
- Test commit: `44ad0d435d501efc2b937b6083e04f3551884c33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 12.4 | 7 | 7 | [run](https://argusic.com/run/bbd05af6-e36c-4ea0-b2af-fa26984faebc) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed`
- 1 min: `pnpm not available on PATH`
- `Git submodules not initialized`
- 5 min: `Missing GTK/WebKit dev libraries (glib, gtk3, webkit2gtk-4.1, pango, cairo, etc.)`
- 2 min: `Missing runtime shared libraries for linking (harfbuzz, cairo-gobject, libxslt, gstreamer, etc.)`
- 2 min: `Node 18.19.1 too old for Vite 7 (crypto.hash not a function)`
- 1 min: `esbuild native binary not built (pnpm ignored build scripts)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
