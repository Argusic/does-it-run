# cheap-ag

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/muaaz9329/cheap-ag, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cheap-ag

## Pinned environment

- Project commit: `d4a8a52b9bb53d2ed6342517c4524e7be4944c9e`
- Test commit: `d4a8a52b9bb53d2ed6342517c4524e7be4944c9e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 6.7 | 2 | 2 | [run](https://argusic.com/run/877035fd-696a-4b4b-a4be-902a7e6282b7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 < required >=20.11.1`
- 2 min: `lsof binary not found in container (ENOENT)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
