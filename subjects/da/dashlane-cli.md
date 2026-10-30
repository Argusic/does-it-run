# dashlane-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Dashlane/dashlane-cli, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dashlane-cli

## Pinned environment

- Project commit: `5c812931d8db0ff6dcc3a2b7e1f90d5dac1a527b`
- Test commit: `5c812931d8db0ff6dcc3a2b7e1f90d5dac1a527b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2 to 2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 2 | 2 | 2 | [run](https://argusic.com/run/77df94bb-2eaf-45c7-befb-7c5424827c76) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node v18.19.1 does not meet project requirement of >=22`
- `yarn command not found in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
