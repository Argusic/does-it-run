# fora

**Verdict: runs with mocks.** Argusic Score 89.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ImFeH2/fora, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/fora

## Pinned environment

- Project commit: `f19b93058c737281b24e1d8fc07e6226d0644970`
- Test commit: `f19b93058c737281b24e1d8fc07e6226d0644970`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 22 to 22 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 89.14 | 22 | 22 | 7 | 6 | [run](https://argusic.com/run/a470c65a-d0d6-43e1-b365-8a3881d70a24) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `rustc/cargo not found in container`
- 1 min: `pnpm not found`
- 1 min: `uv not found`
- 2 min: `Node.js 18 too old for Vite (needs 20+)`
- 1 min: `.npmrc prefix setting conflicts with nvm`
- 3 min: `WebUI tests: 10 failures because CloseEvent undefined in default node environment`
- `Python tests: 7 failures all due to missing bubblewrap sandbox`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
