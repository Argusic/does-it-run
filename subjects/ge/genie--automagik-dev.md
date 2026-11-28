# genie

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/automagik-dev/genie, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/3ca4e2c4-193f-4e8c-abaf-88a000580ae6

## Pinned environment

- Project commit: `6a1e7029c2de43c2cbc1ba778a4a2902de38aca4`
- Test commit: `6a1e7029c2de43c2cbc1ba778a4a2902de38aca4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 38.4 to 38.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 4 | 38.4 | 3 | 0 | [run](https://argusic.com/run/3ca4e2c4-193f-4e8c-abaf-88a000580ae6) |

## What was observed on a clean machine

Attempt 1:

- `36-37 pre-existing flaky test failures in installer promotion/transaction tests (vary between runs, pass individually)`
- `knip dead-code analysis fails on Node.js v18 (lacks node:util.styleText)`
- `One Biome complexity warning (pre-existing, score 26 exceeds threshold 25)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
