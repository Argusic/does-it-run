# codex-command-center

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sevensir888/codex-command-center, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codex-command-center

## Pinned environment

- Project commit: `8aa9baa7bd088ca5e6a4ebf26d8257149a09fce1`
- Test commit: `8aa9baa7bd088ca5e6a4ebf26d8257149a09fce1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 3.2 | 3 | 3 | [run](https://argusic.com/run/9b5c1e03-2583-4180-a9e2-21a40c6c76c6) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm run dev: EMFILE container file-watcher limit`
- 0.5 min: `Rust/Cargo not installed`
- 2 min: `Tauri build and Rust tests fail: missing glib-2.0, libwebkit2gtk, GTK -dev system packages (no root access)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
