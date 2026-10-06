# email-builder-js

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/usewaypoint/email-builder-js, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/email-builder-js

## Pinned environment

- Project commit: `ce3e610749fc80d7e999b20e28f6e775bfe09da7`
- Test commit: `ce3e610749fc80d7e999b20e28f6e775bfe09da7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 5.3 | 3 | 3 | [run](https://argusic.com/run/6d9e0e02-197a-40f5-9a9d-737e6ad419e0) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Duplicate jest.config.js from stale compiled output, causing 'Multiple configurations found' error`
- 1 min: `Stale .js/.d.ts/.map files in packages/*/src/ caused Jest 'Unexpected token' errors (ESM imports in .js files)`
- 0.5 min: `No pre-built dist/ directories in workspace packages, causing TS2307 'Cannot find module'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
