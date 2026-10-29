# env-ci

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/semantic-release/env-ci, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/env-ci

## Pinned environment

- Project commit: `4df63c629e475993f149cf9ce0c9e7524fa149ff`
- Test commit: `4df63c629e475993f149cf9ce0c9e7524fa149ff`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.1 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 2.1 | 2 | 2 | [run](https://argusic.com/run/91489f7f-1a71-42f9-9378-776c58a1ab09) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `System Node v18.19.1 too old for dev dependencies (ava@8, c8@12, etc. require node≥20/≥22). npm install emits EBADENGINE warnings but succeeds with 187 packages.`
- 0.5 min: `Tests fail with 'git commit: Author identity unknown' (4 git-helper failures).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
