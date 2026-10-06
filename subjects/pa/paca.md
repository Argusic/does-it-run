# paca

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Paca-AI/paca, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/paca

## Pinned environment

- Project commit: `839c532ca45183db136569de55cdf5fae4e3fd40`
- Test commit: `839c532ca45183db136569de55cdf5fae4e3fd40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 28 | 6.4 | 5 | 5 | [run](https://argusic.com/run/8b0227ad-515f-4583-b621-0ba435d3f81b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install failed with 'Cannot read properties of null (reading edgesOut)' , Arborist peer dependency resolution crash on Node 18`
- 6 min: `jsdom@29.1.1's html-encoding-sniffer dep uses require() on @exodus/bytes (ESM-only), which throws ERR_REQUIRE_ESM on Node 18`
- 3 min: `vitest@4.x uses rolldown which imports from node:util (Node 22+ only), crashing on startup`
- 5 min: `@blocknote/core/dist uses Array.toReversed() (Node 22+ API) , crashes with 'not a function or its return value is not iterable'`
- `apps/web: @tailwindcss/oxide-linux-x64-gnu native binding missing , npm optional dep resolution bug on this platform`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
