# AstrLink

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Calcium-Ion/AstrLink, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/astrlink

## Pinned environment

- Project commit: `3779884c67d9d7acd9ab921430ae885d906affed`
- Test commit: `3779884c67d9d7acd9ab921430ae885d906affed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 17.8 to 32 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 17.8 | 5 | 5 | [run](https://argusic.com/run/5c171a78-cdd2-4def-bf5c-b8ab10022007) |
| 2 | pass with mocks | 92 | 26 | 32 | 5 | 5 | [run](https://argusic.com/run/6fa61ace-23da-42cb-a43a-be99af5b92be) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Bun requires unzip which was not installed`
- 2 min: `Go not found`
- `Ruby not found for contracts/validate.rb`
- `Desktop Tauri needs glib-2.0 system library`
- 2 min: `Core dies when stdin pipe closes after reading start tokens`

Attempt 2:

- 3 min: `No Go, Rust, or Bun toolchains installed in container`
- 3 min: `ONNX Runtime v1.23.2 LICENSE HTTP 404 from raw.githubusercontent.com`
- 2 min: `Rust 1.88 too old for notify-rust crate (requires 1.89)`
- 1 min: `Ruby not found for contracts/validate.rb`
- `Desktop Tauri Rust crate cannot compile without system-level dev libraries (glib-2.0, webkit2gtk-4.1, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
