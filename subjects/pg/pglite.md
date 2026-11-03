# pglite

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/electric-sql/pglite, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pglite

## Pinned environment

- Project commit: `ae182ff8bd5ba4acb887d6c925d607a1498aa0b5`
- Test commit: `ae182ff8bd5ba4acb887d6c925d607a1498aa0b5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.2 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 5.2 | 0 | 0 | [run](https://argusic.com/run/e68c5efe-bcf3-4746-8d19-41cc37061198) |
| 2 | pass | 100 | 10 | 9.8 | 4 | 4 | [run](https://argusic.com/run/58132722-1dba-4313-90e5-57584fbadc67) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js 18 too old (required >=20)`
- `pnpm not installed`
- 1 min: `release/ dir missing (WASM binaries built via Docker, not available)`
- `Missing pglite.data file in dist/ and release/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
