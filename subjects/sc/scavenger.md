# Scavenger

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rndinfosecguy/Scavenger, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/scavenger

## Pinned environment

- Project commit: `4d3b0ed7e9fb26eec01bc6c0a01e343b08632f11`
- Test commit: `4d3b0ed7e9fb26eec01bc6c0a01e343b08632f11`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 5 | 2 | 2 | [run](https://argusic.com/run/9cdff813-5f74-44c5-9b82-d8caf5ee40d4) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `tmux not installed (no root)`
- 0.1 min: `data directories named pastesoi instead of pastesio`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
