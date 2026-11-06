# better-sqlite3

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WiseLibs/better-sqlite3, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/better-sqlite3

## Pinned environment

- Project commit: `f8e2d541208281368129929a96f70f937c0735ef`
- Test commit: `f8e2d541208281368129929a96f70f937c0735ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 12.6 | 1 | 1 | [run](https://argusic.com/run/b934bfe1-431a-4823-b40d-2388d0ed0e2a) |
| 2 | pass | 100 | 4 | 2 | 2 | 2 | [run](https://argusic.com/run/599370db-9e80-476e-bd72-0fed4df07cc1) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Test timeout for 'anonymous temporary databases' on first run (mocha timeout at 5000ms)`

Attempt 2:

- 2 min: `System Node.js v18.19.1 does not satisfy engines "node": ">=22"`
- 1 min: `Mistakenly overwrote the Node SHASUMS256.txt file during download (self-inflicted)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
