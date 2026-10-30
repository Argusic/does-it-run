# Uni-CLI

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/olo-dot-io/Uni-CLI, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/uni-cli

## Pinned environment

- Project commit: `aed1a389b74818de22c3eb2593f4fd5dac016989`
- Test commit: `aed1a389b74818de22c3eb2593f4fd5dac016989`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20 to 20 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 42 | 20 | 1 | 1 | [run](https://argusic.com/run/03f26bd1-646a-4a70-ae7b-77e9f5628829) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System node v18.19.1 is below the project minimum v22.19 , npm install, build, and tests all fail without a compatible Node`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
