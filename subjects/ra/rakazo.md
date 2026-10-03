# rakazo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elie222/rakazo, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/rakazo

## Pinned environment

- Project commit: `ed2cfb5cafa24d045f32e00e3e8fd80754fbef38`
- Test commit: `ed2cfb5cafa24d045f32e00e3e8fd80754fbef38`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.9 to 21.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 21.8 | 3 | 3 | [run](https://argusic.com/run/add539a3-4686-4a03-acf0-11e70f9fcce1) |
| 2 | pass | 100 | 9 | 8.9 | 0 | 0 | [run](https://argusic.com/run/f8c429f3-0838-40dc-94c6-294b0172cba8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18 pre-installed, project requires >=22.22.2`
- 1 min: `pnpm not pre-installed`
- 1 min: `npm global install blocked by EACCES due to project .npmrc prefix override`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
