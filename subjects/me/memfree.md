# memfree

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/memfreeme/memfree, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/memfree

## Pinned environment

- Project commit: `3163843f3475e767d0a6154ab20462f12cbb82dc`
- Test commit: `3163843f3475e767d0a6154ab20462f12cbb82dc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 16.9 to 20.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 20.4 | 0 | 0 | [run](https://argusic.com/run/82c6105b-cfd3-4396-a851-844ccc667fdf) |
| 2 | pass with mocks | 92 | 8 | 16.9 | 4 | 4 | [run](https://argusic.com/run/74084bc7-e7cc-4566-bc48-f50681c9fbd8) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Frontend test 'should update the active search' failed because updateActiveSearch didn't sync changes back to the searches array`
- 2 min: `Vector redis tests require real Upstash Redis (the @upstash/redis SDK uses internal pipeline protocol not compatible with a simple HTTP mock)`
- `6 vector test files import functions (changeEmbedding, createEmptyTable, checkout, deleteUrls, reCreateEmptyTable) that were commented out in db.ts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
