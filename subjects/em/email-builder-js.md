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
- Valid runs: 2; wall time 5.3 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 5.3 | 3 | 3 | [run](https://argusic.com/run/6d9e0e02-197a-40f5-9a9d-737e6ad419e0) |
| 2 | pass | 100 | 25 | 6.5 | 2 | 2 | [run](https://argusic.com/run/39590681-83ea-4a38-991e-9380549c7d6b) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Duplicate jest.config.js from stale compiled output, causing 'Multiple configurations found' error`
- 1 min: `Stale .js/.d.ts/.map files in packages/*/src/ caused Jest 'Unexpected token' errors (ESM imports in .js files)`
- 0.5 min: `No pre-built dist/ directories in workspace packages, causing TS2307 'Cannot find module'`

Attempt 2:

- 15 min: `Root build script (npx tsc) generated .js/.d.ts files in src/ directories, polluting the source tree. ts-jest then resolved to the .js files instead of .tsx files, causing 'Cannot use import statement outside a module' errors on all 26 test`
- 1 min: `Duplicate jest.config.js found alongside jest.config.ts, causing 'Multiple configurations found' error.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
