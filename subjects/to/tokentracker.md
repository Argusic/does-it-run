# TokenTracker

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xiufengsun/TokenTracker, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/tokentracker

## Pinned environment

- Project commit: `0421f06af6a46f77e30493f34fe9da3a8d4f778f`
- Test commit: `0421f06af6a46f77e30493f34fe9da3a8d4f778f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.4 to 26.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 26.4 | 6 | 6 | [run](https://argusic.com/run/a1337f50-476d-4882-966f-76d7142221bb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 does not meet engine requirement >=20; node:sqlite not available`
- 1 min: `node:sqlite built-in module requires --experimental-sqlite flag on Node 22`
- 1 min: `Node 22 cannot import .ts files without --experimental-strip-types flag`
- 1 min: `dashboard/dist/ directory missing, causing init-local-runtime-reinstall test to fail`
- 3 min: `Vite dashboard dependencies not installed (e.g. @vitejs/plugin-react, @testing-library/react), causing vite-pet-api and TS guardrails tests to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
