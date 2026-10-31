# agent-sandbox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mattolson/agent-sandbox, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-sandbox

## Pinned environment

- Project commit: `c5b65e7cbd8f5b3bbf4e3ea40900c0014eedfa04`
- Test commit: `c5b65e7cbd8f5b3bbf4e3ea40900c0014eedfa04`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 4 | 2 | 2 | [run](https://argusic.com/run/34901eaf-dd37-43aa-842d-d5053900d49c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.26.1 compiler not found in container`
- 1 min: `PyYAML module missing for proxy Python tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
