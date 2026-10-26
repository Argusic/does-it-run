# fluid

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/frontvibe/fluid, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/fluid

## Pinned environment

- Project commit: `16ab5c68404ee445ac65575ab0b99528dcce935d`
- Test commit: `16ab5c68404ee445ac65575ab0b99528dcce935d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 7.6 | 3 | 3 | [run](https://argusic.com/run/761110c7-32c3-449b-8a74-4f7b38f041bb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18.19.1 is below required 20.x - Shopify CLI refused to load config`
- 1 min: `@tailwindcss/oxide native binding not found for linux-x64-gnu`
- 1 min: `JavaScript heap out of memory during Vite build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
