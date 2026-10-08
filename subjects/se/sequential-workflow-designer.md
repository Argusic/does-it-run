# sequential-workflow-designer

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nocode-js/sequential-workflow-designer, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/sequential-workflow-designer

## Pinned environment

- Project commit: `842e3b251233a613f2cdbd8785d1523d1b1d1648`
- Test commit: `842e3b251233a613f2cdbd8785d1523d1b1d1648`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.9 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96.67 | 25 | 12.9 | 6 | 5 | [run](https://argusic.com/run/390d701e-b9ee-4cdb-ab82-ed3e3e9c7df1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `ReturnType<typeof setTimeout> type mismatch with TypeScript 4.6.4 (returns Timeout not number)`
- 2 min: `window.structuredClone not recognized by TS lib target`
- 8 min: `karma-typescript-es6-transform incompatible with Babel v7 , missing noIndentInnerCommentsHere()`
- 2 min: `ChromeHeadless needs --no-sandbox flag in container`
- 2 min: `Karma coverage instrumentation fails with Babel v7`
- `Angular and Svelte subproject builds fail (environment deps)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
