# Wireguard-panel

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Azumi67/Wireguard-panel, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/wireguard-panel

## Pinned environment

- Project commit: `08745a1bac5fab57e8653397c2c3f4475630b6bc`
- Test commit: `08745a1bac5fab57e8653397c2c3f4475630b6bc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.8 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 5.8 | 1 | 1 | [run](https://argusic.com/run/c4915395-862b-45ad-bdd3-3e44b840d82d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Flask-Limiter and Flask-Caching configured to require Redis server (not available in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
