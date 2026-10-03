# flint-chart

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/flint-chart, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/flint-chart

## Pinned environment

- Project commit: `683d5de1ffd0c1a76001ca5aa044f297276d7734`
- Test commit: `683d5de1ffd0c1a76001ca5aa044f297276d7734`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 14 | 4 | 4 | [run](https://argusic.com/run/2478592b-a61d-4c80-97a1-e2dc089879a3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `vitest@4.1.10 requires Node ^20 (module 'node:util' does not provide 'styleText')`
- 4 min: `tsup DTS worker runs out of memory with default 512MB heap on Node 18`
- 3 min: `vite@8 uses rolldown which requires Node 20+, blocks MCP UI build`
- 2 min: `vite-plugin-singlefile@2 depends on rolldown transitively via vite 8`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
