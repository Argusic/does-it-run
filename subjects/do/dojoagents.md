# DojoAgents

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Alpha-Dojo/DojoAgents, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/dojoagents

## Pinned environment

- Project commit: `9b3a9ba510840bf991de02fc41070247d001bf2a`
- Test commit: `9b3a9ba510840bf991de02fc41070247d001bf2a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.2 to 23.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 23.2 | 3 | 3 | [run](https://argusic.com/run/cc103e30-40bc-4022-8e73-f29b84d45583) |

## What was observed on a clean machine

Attempt 1:

- 13 min: `test suite: 8 failures on fresh install (dojosdk 0.1.33 schema drift in sector-brief-extract list/write models + pagination, plus HuggingFace kline wire-format change)`
- 1 min: `system uv not installed and Node 18.19.1 too old for Vite 8 build hook`
- 1 min: `dashboard /health route returns 404 (no such route in this app)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
