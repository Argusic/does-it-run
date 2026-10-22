# qdrant-js

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qdrant/qdrant-js, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/qdrant-js

## Pinned environment

- Project commit: `38fe9949cb21451052d1cabab2b9a423b50ca19b`
- Test commit: `38fe9949cb21451052d1cabab2b9a423b50ca19b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 5.4 | 4 | 4 | [run](https://argusic.com/run/7bfa9cbb-7ca4-4a27-9df6-c44d34b27e88) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 was installed but the project requires >=22.13.0`
- 0.5 min: `pnpm was not installed`
- `Build failed on first attempt due to crypto not defined in serialize-javascript under Node 18`
- 1.5 min: `No Qdrant server running for integration tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
