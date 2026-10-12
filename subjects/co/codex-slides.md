# codex-slides

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nexu-io/codex-slides, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codex-slides

## Pinned environment

- Project commit: `dbc2a5992e937760e9ce8e587e11729f970881cb`
- Test commit: `dbc2a5992e937760e9ce8e587e11729f970881cb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 12 | 7.6 | 4 | 3 | [run](https://argusic.com/run/981a7e4f-4a6e-482d-82f2-4c8d16a75ac3) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node 18 (<20 required) plus missing/broken corepack/pnpm toolchain`
- 3 min: `Corepack shim failed to download pnpm (MODULE_NOT_FOUND) and mutated package.json with a packageManager field`
- 2 min: `TS-importing tests failed under Node 20 (ERR_UNKNOWN_FILE_EXTENSION for .ts)`
- 2 min: `Electron desktop cannot start in this rootless container: chrome-sandbox needs root-owned mode 4755; launcher offers no --no-sandbox path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
