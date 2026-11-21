# solomd

**Verdict: runs.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhitongblog/solomd, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/solomd

## Pinned environment

- Project commit: `47d5f2e263cdfe95c5a4731c64cca3fcb3c50f2a`
- Test commit: `47d5f2e263cdfe95c5a4731c64cca3fcb3c50f2a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 13.7 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88 | 11 | 16.2 | 5 | 4 | [run](https://argusic.com/run/f046e893-8c0b-4d4c-be7d-6d8dca889462) |
| 2 | pass | 96 | 8 | 13.7 | 5 | 4 | [run](https://argusic.com/run/e50a22f1-068e-46b6-9661-0cad3de1087a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in PATH`
- 1 min: `pnpm requires approving build scripts for core-js and esbuild`
- 1 min: `GLib/GDK/GIO system .pc files missing for Tauri build`
- 1 min: `Runtime .so symlinks missing for linker`
- 5 min: `Desktop app (SoloMD) linking fails: libdbus-1 on system has _dbus_prefixed symbols instead of dbus_ symbols the Rust dbus crate expects`

Attempt 2:

- 1 min: `pnpm npm global install failed (EACCES)`
- `pnpm ignored build scripts (core-js, esbuild)`
- `test-self.mjs imports pinyin/simplifiedToTraditional/traditionalToSimplified from wrong module (chinese.ts instead of chinese-convert.ts)`
- 25 min: `Tauri desktop app cannot build (no system .deb -dev packages)`
- `Astro web build fails (Node.js 18.19.1 < 18.20.8 required)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
