# ha-tplink-deco

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amosyuen/ha-tplink-deco, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ha-tplink-deco

## Pinned environment

- Project commit: `5d1eafe2f975e09131121518f535a800542c16ab`
- Test commit: `5d1eafe2f975e09131121518f535a800542c16ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6.5 | 7 | 2 | 2 | [run](https://argusic.com/run/cdae2f49-e8a7-47dd-a205-9bc2f7bb517f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System pip install blocked by PEP 668 externally-managed-environment`
- 1 min: `ModuleNotFoundError: No module named 'Crypto'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
