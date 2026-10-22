# better-design

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/marvkr/better-design, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/better-design

## Pinned environment

- Project commit: `e146625f3041ef8089a2013587435fc763dc3b15`
- Test commit: `e146625f3041ef8089a2013587435fc763dc3b15`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 2.9 | 2 | 2 | [run](https://argusic.com/run/e6516363-170e-4ccb-8989-90d4ba5641c2) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `bun is not installed in the container (documented test runner)`
- 9 min: `tests/vitest 5 fails to start on the container's Node 18.19.1 (SyntaxError: node:util does not provide an export named 'styleText')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
