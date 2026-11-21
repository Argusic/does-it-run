# nodepress

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/surmon-china/nodepress, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nodepress

## Pinned environment

- Project commit: `56ed59f3fec216ff9f82a54c00a9dc25f134f71c`
- Test commit: `56ed59f3fec216ff9f82a54c00a9dc25f134f71c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 10 | 5 | 5 | [run](https://argusic.com/run/dd527700-277c-4f5b-9502-45203a7ef45c) |
| 2 | pass | 100 | 12 | 12.4 | 6 | 6 | [run](https://argusic.com/run/a993eff0-1fdf-4f88-9285-51d9d57b06c2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pnpm not available on PATH`
- 2 min: `ERR_PNPM_IGNORED_BUILDS blocking dependency install`
- 2 min: `Build failed with JavaScript heap OOM`
- 3 min: `MongoDB binary not found in container`
- 8 min: `Redis binary not found in container`

Attempt 2:

- 2 min: `Node.js 18.19.1 below engine requirement >=22`
- 1 min: `pnpm install blocked by ERR_PNPM_IGNORED_BUILDS`
- 1 min: `nest build crashed with OOM`
- 1 min: `jest.config.ts import of tsconfig.json failed (ERR_IMPORT_ATTRIBUTE_MISSING)`
- 2 min: `MongoDB not available`
- 4 min: `Redis not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
