# flat

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/netless-io/flat, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/flat

## Pinned environment

- Project commit: `d194d5b0986b0248f799d487a4b56f77e65165c9`
- Test commit: `d194d5b0986b0248f799d487a4b56f77e65165c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 27.8 to 28.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1.5 | 28.7 | 4 | 4 | [run](https://argusic.com/run/a11028f2-df94-4579-9e00-eca13000e120) |
| 2 | pass with mocks | 92 | 0.5 | 27.8 | 2 | 2 | [run](https://argusic.com/run/21354c36-022b-4cc2-b732-e385ce8410cc) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `'pnpm i -g pnpm@9.9.0' failed with EACCES (no write to /usr/local/lib/node_modules)`
- `agora-electron-sdk postinstall script 'genOS.js' threw ReferenceError: logger is not defined (unsupported Linux platform)`
- `flat-web 'vite build' hits OOM (JavaScript heap out of memory) at ~980 MB , only 2 GB RAM available`
- `TypeScript check of flat-web reports 'error TS2307: Cannot find module 'src/types/user'' in flat-components/VideoAvatar`

Attempt 2:

- `agora-electron-sdk postinstall fails on Linux with 'logger is not defined' / 'Unsupported platform!'`
- `vite build (production) OOMs during chunk rendering (~2GB heap insufficient in ~755MB container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
