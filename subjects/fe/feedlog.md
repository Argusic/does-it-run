# feedlog

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/linkcraftstudio/feedlog, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/feedlog

## Pinned environment

- Project commit: `7d760523d3be95c195fd3be2bf547b91a1ac5ce3`
- Test commit: `7d760523d3be95c195fd3be2bf547b91a1ac5ce3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.1 to 14.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 13 | 14.1 | 4 | 3 | [run](https://argusic.com/run/d69d3104-6fc3-4aaa-b608-1b5c66de5492) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 too old for Nuxt 4 (needs 22+)`
- 1 min: `pnpm not installed`
- 5 min: `No PostgreSQL 17+ available; root not available for apt`
- `5 pre-existing test failures: agent-v1 AI visibility test (Organization not found fixture issue), 4 inbox-scheduler help-indexing timing tests (race conditions in scheduler)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
