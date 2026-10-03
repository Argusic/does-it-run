# openwhispr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenWhispr/openwhispr, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/openwhispr

## Pinned environment

- Project commit: `9d9980ae9042caba963d3b18abea1c6692ae701a`
- Test commit: `9d9980ae9042caba963d3b18abea1c6692ae701a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 71.4 to 71.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 71.4 | 5 | 5 | [run](https://argusic.com/run/a7a1dee3-aab0-45dc-9ec9-1d9c1bccff0c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 installed but project requires >=24`
- 20 min: `tsx wraps ESM imports in {default: ...} for CJS test files, breaking destructuring in await import('.ts')`
- `Node --experimental-strip-types does not resolve extensionless relative imports (import './logger' instead of './logger.ts')`
- `JSON imports need import attributes and named exports don't work natively`
- `require('.tsx') for JSX components fails with strip-types`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
