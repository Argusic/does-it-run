# mex

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mex-memory/mex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mex

## Pinned environment

- Project commit: `490ffe5017c6f1abc4f943931f5a683a04b25df7`
- Test commit: `490ffe5017c6f1abc4f943931f5a683a04b25df7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 26.2 to 40.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 40.5 | 0 | 0 | [run](https://argusic.com/run/e388b127-fa51-4edb-86b9-165f025e3b6b) |
| 2 | pass | 100 | 13 | 26.2 | 3 | 3 | [run](https://argusic.com/run/9e5a11ca-eed7-45f4-a828-2c276ef1ffdc) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js v18.19.1 pre-installed but project requires >=22.5`
- 2 min: `Node 22.5.0 official build lacks SQLite FTS5 support`
- `node:sqlite module needs --experimental-sqlite flag in Node 22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
