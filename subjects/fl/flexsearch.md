# flexsearch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nextapps-de/flexsearch, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/flexsearch

## Pinned environment

- Project commit: `f7ed963096a0792da7b2fd63bb7114b3fbac55ed`
- Test commit: `f7ed963096a0792da7b2fd63bb7114b3fbac55ed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12 to 34.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.4 | 12 | 2 | 2 | [run](https://argusic.com/run/3424584e-d5c7-434a-9e53-cfc48d51eb96) |
| 2 | pass | 100 | 0.5 | 34.1 | 1 | 1 | [run](https://argusic.com/run/95323fb7-7856-44dc-b31d-e6f271508ef0) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Root package.json lacked 'type: module' but src/ files use ESM import , tests crashed on SyntaxError when importing from src/bundle.js`
- `Persistent DB tests (persistent.clickhouse.js, persistent.redis.js, etc.) fail because external services (Redis, Clickhouse) are unavailable`

Attempt 2:

- 5 min: `Root package.json lacks "type": "module", causing ES module imports from test/ to src/ to fail with SyntaxError because Node 18 treats .js as CommonJS when no parent package.json declares type=module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
