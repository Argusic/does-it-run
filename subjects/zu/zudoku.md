# zudoku

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zuplo/zudoku, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/zudoku

## Pinned environment

- Project commit: `3e6ad95294bb2ffe9cca8e50c9213c9ca6aaeda7`
- Test commit: `3e6ad95294bb2ffe9cca8e50c9213c9ca6aaeda7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.8 to 25.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 6.8 | 0 | 0 | [run](https://argusic.com/run/f4f12471-6a58-4391-b369-25602dc7b176) |
| 2 | pass | 100 | 15 | 25.4 | 4 | 4 | [run](https://argusic.com/run/52b0af41-99e2-45b6-bf26-f1df10d91f73) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18 provided, needs >=22.22.0`
- 5 min: `Native optional deps not installed by pnpm (oxfmt, rolldown, oxc-parser bindings)`
- 1 min: `@tailwindcss/oxide native binding missing`
- 5 min: `cosmo-cargo:build gets Illegal instruction on AMD EPYC CPU`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
