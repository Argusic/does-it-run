# codegraph

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/colbymchenry/codegraph, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codegraph

## Pinned environment

- Project commit: `6560052a6f856855d3f71eee838fd66ccfa4285d`
- Test commit: `6560052a6f856855d3f71eee838fd66ccfa4285d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11 to 45.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 45.1 | 1 | 1 | [run](https://argusic.com/run/46bc775c-e39c-4d33-a4b1-66d4ef693e9b) |
| 2 | pass | 100 | 10.5 | 11 | 2 | 2 | [run](https://argusic.com/run/a578e656-9328-4cec-969b-82a407f5c1fc) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Container Node.js v18.19.1 does not have node:sqlite (requires >=22.5) , all DB-backed tests fail with 'No such built-in module: node:sqlite'`

Attempt 2:

- 4 min: `System Node.js v18.19.1 too old (requires >=20); install script bundled binary works anyway but source build needs >=22.5`
- `bundle-launcher.test.ts fails because zip utility is not installed (tests call 'zip' to validate release archives)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
