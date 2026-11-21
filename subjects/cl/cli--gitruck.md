# cli

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Gitruck/cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/e2cc45de-9190-4942-a30c-b890e9882fca

## Pinned environment

- Project commit: `13d484fbebb45a8382169eef17c5cf163715d2d3`
- Test commit: `13d484fbebb45a8382169eef17c5cf163715d2d3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 0.3 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 7.5 | 4 | 4 | [run](https://argusic.com/run/e2cc45de-9190-4942-a30c-b890e9882fca) |
| 2 | fail | 20 | n/a | 0.3 | 0 | 0 | [run](https://argusic.com/run/069b08ff-c332-47b1-88ae-3a45059e14b2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 installed but project requires >=20.6`
- 1 min: `Bun not in PATH after npm install -g`
- 1 min: `Test suite unavailable , test/ directory is a private git submodule with no files in the public repo checkout`
- 2 min: `npm test fails , test/*.test.mjs glob matches no files (empty test dir)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
