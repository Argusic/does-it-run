# ZCode

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zai-org/ZCode, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/zcode

## Pinned environment

- Project commit: `29628c9acdb81b703bbd4080c207a0e7ce5e276e`
- Test commit: `29628c9acdb81b703bbd4080c207a0e7ce5e276e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 12.2 to 32.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 32.5 | 0 | 0 | [run](https://argusic.com/run/e1237878-d43a-4a8e-8e23-10cfc0b79a8a) |
| 2 | pass | 100 | 12 | 12.2 | 3 | 3 | [run](https://argusic.com/run/150acdfd-763b-41d7-903c-9ac32c6aaf64) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `System Node.js v18.19.1; project requires v24.14.0`
- 1 min: `pnpm not found on PATH`
- 0.5 min: `node:test cannot load TypeScript source files directly`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
