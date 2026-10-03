# Codex-X

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yynxxxxx/Codex-X, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/codex-x

## Pinned environment

- Project commit: `8f018fddd3ee1a68464e4df8765eb370ede0c76f`
- Test commit: `8f018fddd3ee1a68464e4df8765eb370ede0c76f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 6 | 5 | 5 | [run](https://argusic.com/run/c07fe855-75a5-4172-ba3c-afaef3661a3d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed`
- 2 min: `Rust/Cargo not installed`
- 2 min: `Node.js 18 too old for Vite 7 build (crypto.hash not a function)`
- 1 min: `Tests import .ts files which Node.js 18 can't load natively`
- `Tauri Rust backend build fails , missing system libraries glib-2.0.pc, gtk-3, webkit2gtk, etc.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
