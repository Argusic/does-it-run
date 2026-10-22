# agent-manager

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/YoanWai/agent-manager, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/agent-manager

## Pinned environment

- Project commit: `ecd836fb0c1ca3955162df54abd8bf25581f8ab5`
- Test commit: `ecd836fb0c1ca3955162df54abd8bf25581f8ab5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.1 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 15.1 | 2 | 2 | [run](https://argusic.com/run/71c7fd50-ba34-48d2-9245-9af8b3909a18) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler not installed in container`
- 4 min: `tmux not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
