# sudocode

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sudocode-ai/sudocode, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/sudocode

## Pinned environment

- Project commit: `632de1910bc4e272f99db7a33dad8f22feb743d9`
- Test commit: `632de1910bc4e272f99db7a33dad8f22feb743d9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 35.6 to 35.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 35.6 | 8 | 8 | [run](https://argusic.com/run/9d0a518e-462c-4ba1-8fd1-06cd5739ac91) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npm install failed first pass due to engine-strict=true .npmrc`
- 2 min: `sudocode meta-package bin links break install (ENOENT on chmod dist/cli.js)`
- 1 min: `TypeScript 5.3+ precompiled _tsc.js incompatible with Node 18`
- 2 min: `CLI: @types/node@20.x fetch Response type mismatches Node 18 global fetch; @types/chokidar@1.7 too old for chokidar v4`
- 2 min: `Frontend: @testing-library/jest-dom not installed in workspace; tsc types referenced it`
- 1.5 min: `Server: pre-existing strict typing errors`
- 5 min: `Vitest test runner crashes with bus error (SIGBUS=135) on Node 18`
- 3 min: `Server cannot start due to ESM resolution on Node 18 (async-mutex, iconv-lite)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
