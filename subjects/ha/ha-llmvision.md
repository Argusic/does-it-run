# ha-llmvision

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/valentinfrlch/ha-llmvision, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ha-llmvision

## Pinned environment

- Project commit: `b81d62688f549332194413ae500eed81b313a58e`
- Test commit: `b81d62688f549332194413ae500eed81b313a58e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 59.6 to 59.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 59.6 | 3 | 3 | [run](https://argusic.com/run/c25bf301-f1ac-4104-b04b-88fb72126953) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pytest-homeassistant-custom-component==0.13.296 requires Python >=3.13 (container has 3.12)`
- 1 min: `homeassistant==2025.11.2 does not exist on PyPI (max published is 2025.1.4)`
- 8 min: `coverage==7.10.6 conflicts with pytest-homeassistant-custom-component which requires coverage==7.6.8`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
