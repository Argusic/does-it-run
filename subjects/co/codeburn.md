# codeburn

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/getagentseal/codeburn, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codeburn

## Pinned environment

- Project commit: `500412aa88dc45ddc756a213e8bd2fd63a5bf7aa`
- Test commit: `500412aa88dc45ddc756a213e8bd2fd63a5bf7aa`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 8.4 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 8.6 | 1 | 1 | [run](https://argusic.com/run/1582c114-76e6-43b0-9237-c78ec36e8d3e) |
| 2 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/e041dd47-ced5-4a1e-8d80-957f6e956239) |
| 3 | pass | 100 | 9 | 8.4 | 2 | 2 | [run](https://argusic.com/run/f1f81b12-ca44-4ee9-b806-b57bc25523db) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js version mismatch: repo requires >=22.13.0, system had v18.19.1`

Attempt 3:

- 1 min: `Node.js v18.19.1 is pre-installed but project requires >=22.13.0`
- 2 min: `2 test timeouts in full suite (cli-plan.test.ts / cli-price-override.test.ts)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
