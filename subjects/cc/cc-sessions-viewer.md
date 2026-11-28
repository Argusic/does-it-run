# cc-sessions-viewer

**Verdict: could not verify.** Argusic Score 36 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jerrywu001/cc-sessions-viewer, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/cc-sessions-viewer

## Pinned environment

- Project commit: `c81f59223af22893d2d5da5c77d3b2c3af0a20a3`
- Test commit: `c81f59223af22893d2d5da5c77d3b2c3af0a20a3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6 to 24 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 18 | 6 | 1 | 0 | [run](https://argusic.com/run/79870be4-c6ed-446c-a422-e938f711c96a) |
| 2 | fail | 42 | 22 | 24 | 5 | 3 | [run](https://argusic.com/run/96d337c7-6dd3-414d-9a7d-09ca7d1f2e3f) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Tauri/Rust build: glib-sys crate fails , package 'glib-2.0' not found in pkg-config search path, requires libglib2.0-dev and related -dev packages (libgtk-3-dev, libwebkit2gtk-4.1-dev, libsoup-3.0-dev) which cannot be 'apt-get install'ed wi`

Attempt 2:

- 3 min: `Node v18.19.1 too old for dependency requirements (needs ^20.19.0 / ^22.12.0)`
- 2 min: `Rolldown native binding build for wrong Node version after upgrade`
- 15 min: `Rust build fails: missing glib-2.0, webkit2gtk-4.1, gtk+-3.0, etc. -dev packages (no root)`
- 1 min: `Tauri binary exits with 'Unable to spawn WebKitNetworkProcess' , WebKit runtime subprocesses at /usr/lib/x86_64-linux-gnu/webkit2gtk-4.1/ don't exist and cannot be created without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
