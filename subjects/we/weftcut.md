# WeftCut

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WeftCut/WeftCut, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/weftcut

## Pinned environment

- Project commit: `610061dca1e9e9cc44af3875465dee1321adae8d`
- Test commit: `610061dca1e9e9cc44af3875465dee1321adae8d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31.1 to 31.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 31.1 | 8 | 8 | [run](https://argusic.com/run/5eea6c35-1a0b-46d2-a24a-b10b1f700a4f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 too old (requires >=24)`
- 2 min: `Rust toolchain not installed`
- 1 min: `npmrc ignore-scripts=true blocked optional native bindings`
- 3 min: `napi:build:decode failed - libclang not found`
- 1 min: `ffmpeg-sys-next build failed - libavutil.pc not found`
- 3 min: `clang bindgen failed - limits.h not found`
- `1 vitest test fails - rmSync on symlinked directory (Node 24)`
- `1 script test fails - Playwright Chromium not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
