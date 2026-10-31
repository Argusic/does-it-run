# capri

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/capri-js/capri, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/capri

## Pinned environment

- Project commit: `6242dfa3f69cd87ccf1b15035237a98236d7737f`
- Test commit: `6242dfa3f69cd87ccf1b15035237a98236d7737f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 4.9 | 2 | 2 | [run](https://argusic.com/run/e748a100-25e1-4197-a1da-622ddd4c1d6c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `tsc build failed: missing @types/micromatch declaration file`
- 4 min: `vitest 4.x requires Node >=20, container has Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
