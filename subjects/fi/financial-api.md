# Financial-API

**Verdict: runs with mocks.** Argusic Score 87 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HiThink-Tech/Financial-API, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/financial-api

## Pinned environment

- Project commit: `3bca7805a4127ece8d81961917e740d2effac6ec`
- Test commit: `3bca7805a4127ece8d81961917e740d2effac6ec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.5 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 11 | 11.5 | 4 | 3 | [run](https://argusic.com/run/6a86130f-c3c3-402e-894d-40280615c41a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Bundled vitest 4.x fails on Node 18 (requires ^20.0.0 || ^22.0.0)`
- 1 min: `Direct pip install blocked by PEP 668 externally-managed environment`
- 2 min: `CLI uses import.meta.dirname (Node 21+); crashes on Node 18`
- 1 min: `pytest not installed in venv (opt-dependencies dev omitted)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
