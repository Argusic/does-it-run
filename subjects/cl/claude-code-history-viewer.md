# claude-code-history-viewer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jhlee0409/claude-code-history-viewer, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claude-code-history-viewer

## Pinned environment

- Project commit: `7f48907081d93ad209b30e10ff640ea0b8ed0e24`
- Test commit: `7f48907081d93ad209b30e10ff640ea0b8ed0e24`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 42.8 to 42.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 41 | 42.8 | 6 | 6 | [run](https://argusic.com/run/a56ecf99-b1c4-495a-a778-e3e91db3ab6b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm binary not found in PATH`
- 1 min: `@tailwindcss/oxide-linux-x64-gnu native binding missing in pnpm store`
- 1 min: `Node.js 18.19 too old for Vite 7 (requires 20.19+)`
- 10 min: `System -dev libraries missing (glib, gtk, webkit, etc.) for Rust build`
- 5 min: `Runtime .so libraries missing for server binary (gstreamer, enchant, wayland, dbus, icu, dw, orc, xslt, etc.)`
- 3 min: `pkg-config proto packages (xproto, kbproto, renderproto, etc.) absent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
