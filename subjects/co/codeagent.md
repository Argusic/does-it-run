# codeAgent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Harvil1/codeAgent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/codeagent

## Pinned environment

- Project commit: `e48780be52949dfcf17338025f6beab48ca01428`
- Test commit: `e48780be52949dfcf17338025f6beab48ca01428`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.3 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 6.3 | 3 | 3 | [run](https://argusic.com/run/2ba220b7-25a6-4bde-b9f6-47605ae69875) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install uv failed: externally-managed-environment (Debian)`
- 1 min: `uv not found after install`
- 3 min: `NO_COLOR=1 env var broke Rich ANSI rendering in BridgeConsole.print`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
