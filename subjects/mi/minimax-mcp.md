# MiniMax-MCP

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MiniMax-AI/MiniMax-MCP, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/minimax-mcp

## Pinned environment

- Project commit: `0856b9aef8a9d676bb63bdd6b6426d7b640a3b7a`
- Test commit: `0856b9aef8a9d676bb63bdd6b6426d7b640a3b7a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 1.4 to 1.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.2 | 1.8 | 1 | 1 | [run](https://argusic.com/run/9fe8bba1-445e-467e-8c8d-330fd0e6a893) |
| 2 | pass | 100 | 0.5 | 1.4 | 0 | 0 | [run](https://argusic.com/run/a3b9e9d4-dca4-4889-a330-db632f265755) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Externally-managed Python environment blocked system-wide pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
