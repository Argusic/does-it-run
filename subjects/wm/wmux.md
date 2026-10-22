# wmux

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openwong2kim/wmux, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wmux

## Pinned environment

- Project commit: `40d4b1f56896b62d2df07efb0afe73774fa15e49`
- Test commit: `40d4b1f56896b62d2df07efb0afe73774fa15e49`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.5 to 23.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 23.5 | 3 | 3 | [run](https://argusic.com/run/b23dcbf9-46f6-4163-9adc-c9f486ff0276) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npm install required node >=22, npm >=11 but container had node 18 / npm 9.2`
- 2 min: `test:runtime , 1 test failed: 'paints completed synchronized frames while OpenCode-style output remains active' , Playwright browser not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
