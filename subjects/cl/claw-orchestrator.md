# claw-orchestrator

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Enderfga/claw-orchestrator, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claw-orchestrator

## Pinned environment

- Project commit: `57ba1c95b3b7922fef634341bac540686d76d9bc`
- Test commit: `57ba1c95b3b7922fef634341bac540686d76d9bc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 4.2 | 1 | 1 | [run](https://argusic.com/run/c7f39b83-a5ae-4999-8a64-e7b8b3b360ec) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node 18 pre-installed, project requires >=22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
