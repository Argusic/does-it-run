# mini-macau

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/asdfghj1237890/mini-macau, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mini-macau

## Pinned environment

- Project commit: `1c7bbddf130214e5f092dee4a4cf75916f38c62e`
- Test commit: `1c7bbddf130214e5f092dee4a4cf75916f38c62e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.7 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 13.7 | 3 | 3 | [run](https://argusic.com/run/4c8517ed-f397-45c2-927f-8727bf823cd2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node 18 is below the project's required Node 20+/22+; vitest 4 crashed at startup ('node:util' has no export 'styleText')`
- 3 min: `First install under Node 18 dropped the rolldown optional native binding, so vitest failed with 'Cannot find native binding'`
- 2 min: `npm test initially executed 533 test files including maplibre-gl's own tests (719 failures) because the moved-aside node_modules.node18 folder was picked up by vitest globbing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
