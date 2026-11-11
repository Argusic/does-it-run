# kaogong-shuati

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ERRRC/kaogong-shuati, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/kaogong-shuati

## Pinned environment

- Project commit: `12cf8e73be8fd18f615782e7a5748b0ca7f39ce2`
- Test commit: `12cf8e73be8fd18f615782e7a5748b0ca7f39ce2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.2 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.2 | 5 | 5 | [run](https://argusic.com/run/41884793-c980-4e14-986f-891f06dfbf82) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 (system) does not support node:sqlite; project requires >=22.5`
- 1 min: `node:sqlite requires --experimental-sqlite flag in v22.6.0`
- `test-local-api.mjs, test-local-queries.mjs, test-local-ai.mjs fail because app-assets/tiku_app.db does not exist`
- 1 min: `Tests spawning child server (test-random-practice-count.mjs et al.) did not pass --experimental-sqlite flag`
- 2 min: `test-custom-practice-e2e.mjs used playwright msedge channel which was not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
