# node-red-dashboard

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FlowFuse/node-red-dashboard, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/node-red-dashboard

## Pinned environment

- Project commit: `be2d2c1a9690e26bb897c024b55721e2251b481f`
- Test commit: `be2d2c1a9690e26bb897c024b55721e2251b481f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.4 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 17.4 | 4 | 4 | [run](https://argusic.com/run/53b8fef9-ffe3-4c6c-8690-cf0a856ac2b1) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Default Node.js 18.19.1 is unsupported by locked Mocha 12/Cypress 15 and other tooling; mocha failed with SyntaxError: Unexpected token 'with' and npm emitted EBADENGINE warnings.`
- 1 min: `Initial blank Node-RED flow returned 404 for /dashboard and /dashboard/_setup because no ui-base config node existed.`
- 1 min: `Cypress run modified tracked fixture config files.`
- 2 min: `Isolated Node-RED launch initially failed with node-red: not found, then ignored the plugin until it was installed in that user directory.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
