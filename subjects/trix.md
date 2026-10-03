# trix

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/basecamp/trix, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/trix

## Pinned environment

- Project commit: `d7c1298088d97686273e1459975f2c8bdb296b58`
- Test commit: `d7c1298088d97686273e1459975f2c8bdb296b58`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 6 | 2 | 2 | [run](https://argusic.com/run/0cfe61b1-5605-4d54-a008-e09c13a98fa9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `yarn not found in PATH`
- 1 min: `pretest script fails due to missing Ruby (rake step)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
