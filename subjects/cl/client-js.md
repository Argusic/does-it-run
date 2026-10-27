# client-js

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/massive-com/client-js, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/client-js

## Pinned environment

- Project commit: `d90f2bb47e559d3e349f5d0f35112249591924eb`
- Test commit: `d90f2bb47e559d3e349f5d0f35112249591924eb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 7.5 | 3 | 3 | [run](https://argusic.com/run/cf047a68-4c0b-451e-9bd7-54182892aa18) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm test fails - mocha 12 uses 'with' type import syntax unsupported on Node 18 (no test files exist anyway)`
- 2 min: `npm run build fails - generate step requires Java (no JDK installed) and openapi-generator-cli has ESM compatibility issues on Node 18`
- `npm ci engine warning - yargs-parser@22 needs Node ^20.19.0 but Node 18.19.1 is available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
