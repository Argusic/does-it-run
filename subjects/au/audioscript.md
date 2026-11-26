# AudioScript

**Verdict: could not verify.** Argusic Score 25 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/niyongsheng/AudioScript, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/audioscript

## Pinned environment

- Project commit: `7ca4e3c385b6107075492364a7b7b36a0d1a3736`
- Test commit: `7ca4e3c385b6107075492364a7b7b36a0d1a3736`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 8.6 to 22.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 22 | 22.2 | 1 | 0 | [run](https://argusic.com/run/6e71d71d-5427-4663-aa64-406c1997c446) |
| 2 | fail | 20 | n/a | 8.6 | 0 | 0 | [run](https://argusic.com/run/28f3843b-4b63-40d5-ae6e-18e02c103e47) |

## What was observed on a clean machine

Attempt 1:

- 22 min: `Rust/Tauri build requires system dev packages (libwebkit2gtk-4.1-dev, libgtk-3-dev, libglib2.0-dev, libpipewire-0.3-dev, libclang-dev, libllvm18 and many transitive -dev deps) that need root to install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
