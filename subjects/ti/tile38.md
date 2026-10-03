# tile38

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tidwall/tile38, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/tile38

## Pinned environment

- Project commit: `a9f953e358d31bc8fc9479ad71f132b1ed752b4b`
- Test commit: `a9f953e358d31bc8fc9479ad71f132b1ed752b4b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.4 to 15.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 15.4 | 1 | 1 | [run](https://argusic.com/run/aa50265a-e4c1-40f9-8191-8f47d1c2114d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `git describe --tags failed: no tags found in repo`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
