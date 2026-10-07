# open-edit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/veedstudio/open-edit, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-edit

## Pinned environment

- Project commit: `dd7913b0bb12c19c5196332df5aff1f55799b291`
- Test commit: `dd7913b0bb12c19c5196332df5aff1f55799b291`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.6 | 3 | 3 | [run](https://argusic.com/run/e7b04b50-96c1-40a9-bb92-e546cb1d4f28) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18.19.1 requires >=20; installing Node v20.18.1`
- 1 min: `pnpm not on PATH; project requires pnpm@10.16.1`
- 1 min: `CLI dist not built (no cli/dist/)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
