# solomd

**Verdict: runs with mocks.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhitongblog/solomd, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/solomd

## Pinned environment

- Project commit: `47d5f2e263cdfe95c5a4731c64cca3fcb3c50f2a`
- Test commit: `47d5f2e263cdfe95c5a4731c64cca3fcb3c50f2a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.2 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88 | 11 | 16.2 | 5 | 4 | [run](https://argusic.com/run/f046e893-8c0b-4d4c-be7d-6d8dca889462) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in PATH`
- 1 min: `pnpm requires approving build scripts for core-js and esbuild`
- 1 min: `GLib/GDK/GIO system .pc files missing for Tauri build`
- 1 min: `Runtime .so symlinks missing for linker`
- 5 min: `Desktop app (SoloMD) linking fails: libdbus-1 on system has _dbus_prefixed symbols instead of dbus_ symbols the Rust dbus crate expects`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
