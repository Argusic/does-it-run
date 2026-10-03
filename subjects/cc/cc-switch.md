# cc-switch

**Verdict: could not verify.** Argusic Score 65 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/farion1231/cc-switch, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/cc-switch

## Pinned environment

- Project commit: `db41d701879592b8eca938cbe5c5ac28dd732b9f`
- Test commit: `db41d701879592b8eca938cbe5c5ac28dd732b9f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 36.1 to 41.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 41 | 41.5 | 1 | 1 | [run](https://argusic.com/run/a1022047-f25a-4d40-b433-443a3c061285) |
| 2 | fail | 50 | 35 | 36.1 | 6 | 6 | [run](https://argusic.com/run/a301cdb3-abe0-4078-89ea-d8795e30c545) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `Rust/Tauri backend cannot compile: missing system dev packages (webkit2gtk-4.1-dev, libgtk-3-dev, etc.) - no root access to apt-get install`

Attempt 2:

- 1 min: `No Rust installed (required for Tauri backend)`
- 1 min: `No pnpm installed`
- 12 min: `Missing system -dev packages: libglib2.0-dev, libgtk-3-dev, libwebkit2gtk-4.1-dev, libsoup-3.0-dev, and 50+ transitive -dev packages`
- 3 min: `Rust linker (rust-lld) could not find shared libraries at link time`
- 5 min: `Rust test binary failed at runtime: missing libxslt.so.1, libgstallocators, libdw, etc.`
- 5 min: `Desktop app (cc-switch) crashes at launch: WebKitNetworkProcess not found at hardcoded /usr/lib/x86_64-linux-gnu/webkit2gtk-4.1/ path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
