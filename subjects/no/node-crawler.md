# node-crawler

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bda-research/node-crawler, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/node-crawler

## Pinned environment

- Project commit: `29d547e3423821088968cf44a784ebd68bde86d3`
- Test commit: `29d547e3423821088968cf44a784ebd68bde86d3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 3.9 | 1 | 1 | [run](https://argusic.com/run/ef6485a3-5c10-4742-ae19-9049ce2a38b1) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `System Node.js is v18.19.1 but package requires >=22. npm install emitted EBADENGINE warnings on many dependencies.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
