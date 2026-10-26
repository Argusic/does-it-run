# http-request-action

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fjogeleit/http-request-action, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/http-request-action

## Pinned environment

- Project commit: `f98bb26551cd1af7d3eb2674578a80754ece88db`
- Test commit: `f98bb26551cd1af7d3eb2674578a80754ece88db`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.8 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 5.8 | 4 | 4 | [run](https://argusic.com/run/6e28fb61-1d39-4cf8-92bd-edf340f5944f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18 in container (package.json requires >=24). npm install succeeded with EBADENGINE warnings.`
- 2 min: `yargs@18 (ESM-only) not compatible with Node 18 require(). CLI failed to load.`
- 2 min: `CLI script called request() without await, so process exited before HTTP request completed.`
- 2 min: `npm run build failed: @vercel/ncc@0.44.1 throws 'N.hash is not a function' on Node 18.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
