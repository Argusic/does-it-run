# agentsilex

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/howl-anderson/agentsilex, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agentsilex

## Pinned environment

- Project commit: `cd529f2838151fd8a4f0d6b7054a45d829b3f78d`
- Test commit: `cd529f2838151fd8a4f0d6b7054a45d829b3f78d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 1.7 to 10.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10.9 | 0 | 0 | [run](https://argusic.com/run/6ce65438-27af-4c29-b05e-3598ecd9e76a) |
| 2 | pass | 100 | 1.2 | 1.7 | 1 | 1 | [run](https://argusic.com/run/e49bed62-78c5-4635-8bbd-cf188ec27213) |

## What was observed on a clean machine

Attempt 2:

- 0.1 min: `mcp.py used attribute 'inputSchema' (camelCase) but the installed mcp-types library exposes it as 'input_schema' (snake_case), causing AttributeError in 3 tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
