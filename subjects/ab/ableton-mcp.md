# ableton-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ahujasid/ableton-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ableton-mcp

## Pinned environment

- Project commit: `9dddc7bd5b95412510fdeb745949e3bf23f3fd8a`
- Test commit: `9dddc7bd5b95412510fdeb745949e3bf23f3fd8a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 4.9 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 4.9 | 0 | 0 | [run](https://argusic.com/run/c8fd7e2f-f040-4640-893e-37618f140144) |
| 2 | pass with mocks | 92 | 2 | 5.3 | 2 | 2 | [run](https://argusic.com/run/73b9fe47-b189-4230-8514-5457383a8efc) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `uv not available in container`
- 1 min: `pytest not in project dependencies`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
