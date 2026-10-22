# claude-brain

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/memvid/claude-brain, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claude-brain

## Pinned environment

- Project commit: `5df71f77aafa4ec50e7fd4672997b6da7e2c3198`
- Test commit: `5df71f77aafa4ec50e7fd4672997b6da7e2c3198`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 8.4 | 1 | 1 | [run](https://argusic.com/run/1928e433-a2e5-4787-8230-829643d696c6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `smart-install.js hook crashed at runtime: __dirname is not defined in ES module scope`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
