# dockit

**Verdict: runs.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/geek-fun/dockit, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dockit

## Pinned environment

- Project commit: `a1556b699a9a04866de39820078dbf05b1173833`
- Test commit: `a1556b699a9a04866de39820078dbf05b1173833`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 10.2 to 12.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 12.5 | 1 | 1 | [run](https://argusic.com/run/371aa190-32f0-40ed-b5c0-da037bdfa1dd) |
| 2 | fail | 0 | 15 | 10.2 | 1 | 0 | [run](https://argusic.com/run/ee7c6852-c8bf-409c-b9ee-3a86b4a2c175) |

## What was observed on a clean machine

Attempt 1:

- `Rust backend cannot compile: system libraries glib-2.0-dev, libwebkit2gtk-4.0-dev not found (no root)`

Attempt 2:

- `Rust backend (Tauri) cannot compile: system library glib-2.0 (-dev headers) not found in pkg-config, requiring libglib2.0-dev, libwebkit2gtk-4.1-dev, libsoup-3.0-dev and other GTK/WebKit dev packages that cannot be installed without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
