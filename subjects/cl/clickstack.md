# ClickStack

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ClickHouse/ClickStack, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/clickstack

## Pinned environment

- Project commit: `0262822da3bb638dc5fc8cbb2105ced6ba0c25ce`
- Test commit: `0262822da3bb638dc5fc8cbb2105ced6ba0c25ce`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.6 to 15.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.5 | 15.6 | 2 | 2 | [run](https://argusic.com/run/49e9395b-bc9c-414b-a214-3d7ae9752c99) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Default Node.js v18.19.1 doesn't support Array.prototype.toSorted() used in packages/app/src/components/DBSearchPageFilters.tsx`
- `Docker not available in container - cannot start ClickHouse, MongoDB, or OTel collector for integration/E2E tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
