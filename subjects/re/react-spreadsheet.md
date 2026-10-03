# react-spreadsheet

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iddan/react-spreadsheet, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-spreadsheet

## Pinned environment

- Project commit: `bb80b60b82981527d5172ce8268af61a517f7e46`
- Test commit: `bb80b60b82981527d5172ce8268af61a517f7e46`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.8 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 3.8 | 1 | 1 | [run](https://argusic.com/run/b537a46a-e122-4871-951f-eaa5c06cf412) |
| 2 | pass | 100 | 2 | 4.1 | 3 | 3 | [run](https://argusic.com/run/49c03772-c72c-49de-94b2-39513fede199) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `rollup.config.mjs used 'import pkg from './package.json' with { type: 'json' }' which requires Node 20+ (container has Node 18.19.1)`

Attempt 2:

- `yarn not found in container`
- 1 min: `npm install ERESOLVE peer dependency conflict between @typescript-eslint/eslint-plugin@6 and eslint-config-react-app@6`
- `rollup.config.mjs uses JSON import assertion 'with { type: "json" }' which requires Node 20+; container has Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
