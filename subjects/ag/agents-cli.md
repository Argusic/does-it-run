# agents-cli

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google/agents-cli, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agents-cli

## Pinned environment

- Project commit: `5597738f14b5d4a490dfdefa282bc229003b7bbe`
- Test commit: `5597738f14b5d4a490dfdefa282bc229003b7bbe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 9.7 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.68 | 9.7 | 3 | 3 | [run](https://argusic.com/run/a71c7c86-e9dc-49b4-bf73-916cb305bd1e) |
| 2 | pass with mocks | 92 | 10 | 13.7 | 0 | 0 | [run](https://argusic.com/run/5b055370-fbe0-4314-84c7-77779c4421c5) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `uv not found on PATH; agents-cli install requires it`
- 0.3 min: `System Python environment is externally managed (PEP 668), blocking pip install of google-agents-cli`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
