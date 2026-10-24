# node-request-retry

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FGRibreau/node-request-retry, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/node-request-retry

## Pinned environment

- Project commit: `9d61cb22310bdafe8cf49e4cc56d66e5c16d69f8`
- Test commit: `9d61cb22310bdafe8cf49e4cc56d66e5c16d69f8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.3 to 3.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 3.3 | 3 | 3 | [run](https://argusic.com/run/960f838a-32a1-461a-a9ca-600e0812cdf4) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install printed EBADENGINE warning for transitive dep walk-up-path@4.0.0 (requires node >=20, container has node 18.19.1); install still completed`
- 1 min: `npm install audit reported 19 vulnerabilities (8 high, 1 critical) in the dependency tree`
- 1 min: `npm run test-coverage printed a Browserslist stale caniuse-lite cache notice`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
