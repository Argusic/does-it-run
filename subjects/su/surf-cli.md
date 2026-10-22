# surf-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nicobailon/surf-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/surf-cli

## Pinned environment

- Project commit: `f7792899abfac4eaa83929a443cf49d011d4a471`
- Test commit: `f7792899abfac4eaa83929a443cf49d011d4a471`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18.8 to 18.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17.5 | 18.8 | 2 | 2 | [run](https://argusic.com/run/ec5c63f8-fdca-4ffc-9670-9d362d1cb74e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18 is too old for rolldown/vite 8 which require node:util.styleText`
- 5 min: `test/unit/pi-extension.test.ts and test/unit/pi-external-job-contract.test.ts used require() to load a TypeScript ESM file containing 'as' type assertions, which Node's CJS loader cannot parse`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
