# omnilogue

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jhlee0409/omnilogue, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/omnilogue

## Pinned environment

- Project commit: `bc50501397f9db38a8f1c535e3d934e80e904828`
- Test commit: `bc50501397f9db38a8f1c535e3d934e80e904828`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 33.6 to 40 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 80 | 10 | 40 | 5 | 2 | [run](https://argusic.com/run/d51fb653-64b2-4ae1-96fb-96f234ee7144) |
| 2 | pass with mocks | 92 | 3.5 | 33.6 | 4 | 4 | [run](https://argusic.com/run/6bd842f6-0be8-4d52-8524-eee89a02c938) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `No root access: missing system packages libglib2.0-dev, libwebkit2gtk-4.1-dev, libgtk-3-dev, libayatana-appindicator3-dev, librsvg2-dev prevent Rust/Tauri build`
- 5 min: `Node.js v18.19.1 was system-installed (needs 20.19+ or 22.12+); upgraded to v22.14.0 via binary download`
- 2 min: `pnpm not in PATH initially; installed to ~/.npm-global/bin`
- 2 min: `Rust not installed; installed via rustup`
- `Full vitest suite hangs when all 400+ test files run together (vitest 4.x fork pool issue); all files pass when run in batches`

Attempt 2:

- 2 min: `Node.js v18 installed, project requires v22.18+ per .nvmrc`
- 1.5 min: `pnpm not in PATH (npm install -g fails EACCES)`
- 0.5 min: `@tailwindcss/oxide-linux-x64-gnu native binding missing`
- `Rust/Tauri build fails - missing GTK/WebKit system libraries`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
