# aeon

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aeonfun/aeon, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/aeon

## Pinned environment

- Project commit: `531f575eb2beaf12d71e8d9699ce451887babdb4`
- Test commit: `531f575eb2beaf12d71e8d9699ce451887babdb4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.4 | 4 | 2 | 2 | [run](https://argusic.com/run/fac33218-897b-4766-bc2e-7850301b2fd2) |
| 2 | pass | 100 | 4.5 | 7.1 | 2 | 2 | [run](https://argusic.com/run/bb5c0819-15a4-4abc-a213-a758d0f600b3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Dashboard test glob 'lib/**/*.test.mjs' not expanded by Node 18 --test runner`
- 1 min: `Webhook worker.js uses ESM import but package.json had no 'type': 'module'`

Attempt 2:

- 2 min: `Webhook package.json missing 'type': 'module' , src/worker.js uses import but node loaded it as CJS`
- 3 min: `Dashboard test glob lib/**/*.test.mjs not expanded by sh , npm test failed to find any test files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
