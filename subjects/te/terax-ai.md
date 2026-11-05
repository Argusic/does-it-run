# terax-ai

**Verdict: runs.** Argusic Score 95.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crynta/terax-ai, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/terax-ai

## Pinned environment

- Project commit: `bc6607c52bdaf9a035ebc8fa87424dc6ddbfcc0c`
- Test commit: `bc6607c52bdaf9a035ebc8fa87424dc6ddbfcc0c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.8 to 16.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 7 | 6.8 | 5 | 4 | [run](https://argusic.com/run/83df2c51-dbf6-463b-9063-4a2fb6062070) |
| 2 | pass | 95 | 16 | 16.9 | 4 | 3 | [run](https://argusic.com/run/1cdf938f-690e-480c-805b-64c49e2d85cf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18.19.1 below project minimum of 22`
- 1 min: `pnpm not found`
- 1 min: `Rust toolchain not found`
- 1 min: `Rolldown native binding missing for Linux x64-gnu`
- `Tauri backend: missing system dev libraries (glib-2.0-dev, libwebkit2gtk-4.1-dev, libsoup-3.0-dev)`

Attempt 2:

- 3 min: `Node.js v18.19.1 installed but project requires >=22`
- 1 min: `pnpm not found in PATH and global npm install blocked by permissions`
- 1 min: `vitest crashed: rolldown uses node:util.styleText unavailable in Node 18`
- `Rust Tauri build requires libglib2.0-dev, libwebkit2gtk-4.1-dev, libsoup-3.0-dev and other dev packages; no root access to install them`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
