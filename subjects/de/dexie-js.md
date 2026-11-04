# Dexie.js

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dexie/Dexie.js, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dexie-js

## Pinned environment

- Project commit: `57a028d7c0ee295c9b1bbfd2e3ea26ed24858fd3`
- Test commit: `57a028d7c0ee295c9b1bbfd2e3ea26ed24858fd3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.4 to 24.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10.5 | 12.4 | 3 | 3 | [run](https://argusic.com/run/e37ae848-699a-4cc6-acf4-fb9c6ec7a9e1) |
| 2 | pass | 100 | 22.8 | 24.2 | 3 | 3 | [run](https://argusic.com/run/ab04c88a-a47b-41c5-82df-90e0a9d821e0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found on PATH`
- 3 min: `just-build v0.9.24 whichLocal misparses pnpm v10+ shell shims, picks up 'elif' as binary path`
- 3 min: `No Chromium/Chrome browser installed`

Attempt 2:

- 15 min: `just-build tool incompatible with pnpm v12 shell shims (elif parsing bug in whichLocal.js)`
- 5 min: `Karma test suite disconnects after ~6.8s of execution (10 test modules pass, then Chrome closes)`
- 2 min: `Chrome for Testing binary downloaded separately (no system browser available, no root access)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
