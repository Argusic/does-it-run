# fast-gateway

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BackendStack21/fast-gateway, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/fast-gateway

## Pinned environment

- Project commit: `f79ca8b0af78b34aa1673ce696caa3f87def2cf5`
- Test commit: `f79ca8b0af78b34aa1673ce696caa3f87def2cf5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 3.4 | 2 | 2 | [run](https://argusic.com/run/5783421d-a9db-4bd0-9bfd-42ce1f1138e1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install failed because @playwright/browser-chromium requires Node.js 20+`
- 0.1 min: `rm -rf node_modules rejected by security sandbox`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
