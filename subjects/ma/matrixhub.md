# matrixhub

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/matrixhub-ai/matrixhub, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/matrixhub

## Pinned environment

- Project commit: `d540d926a72ad985e3299bc66c5ea3a5f10ac673`
- Test commit: `d540d926a72ad985e3299bc66c5ea3a5f10ac673`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10.8 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.8 | 5 | 5 | [run](https://argusic.com/run/ec5394e5-3c15-4813-99a7-96bc56449745) |
| 2 | pass | 100 | 10.5 | 11.3 | 4 | 4 | [run](https://argusic.com/run/6df0debd-6ed4-4810-9d1d-7972942c7ffc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.23+ not pre-installed in container`
- 1 min: `Node.js 18 pre-installed, but Vite requires 20+`
- 0.5 min: `pnpm not pre-installed`
- 0.5 min: `UI build initially failed due to Node 18 with Vite 7`
- `internal/apiserver/handler/hf tests fail (nil pointer in HF handler)`

Attempt 2:

- 1.5 min: `Go compiler not installed`
- 2 min: `pnpm not installed`
- 1.5 min: `Node.js 18.19.1 too old for Vite 7 (requires 20+)`
- `internal/apiserver/handler/hf tests fail (EOF / connection refused)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
