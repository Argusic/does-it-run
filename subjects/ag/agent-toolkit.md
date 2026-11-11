# agent-toolkit

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/softaworks/agent-toolkit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-toolkit

## Pinned environment

- Project commit: `3027f20f3181758385a1bb8c022d4041dfb4de84`
- Test commit: `3027f20f3181758385a1bb8c022d4041dfb4de84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4 | 0 | 0 | [run](https://argusic.com/run/c7a27ffb-58d6-4c80-b465-64c55c90f434) |
| 2 | pass | 80 | 2.3 | 2.4 | 1 | 0 | [run](https://argusic.com/run/2fe1b6aa-1cbe-4939-a527-b7f3c1f87d6e) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `npx skills add softaworks/agent-toolkit failed: Node v18.19.1 below required >=22.20.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
