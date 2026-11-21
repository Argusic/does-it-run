# TikHub-API-Python-SDK

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TikHub/TikHub-API-Python-SDK, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/tikhub-api-python-sdk

## Pinned environment

- Project commit: `2d92927332e1ff0fdc2d05b46381218a0f5a3511`
- Test commit: `2d92927332e1ff0fdc2d05b46381218a0f5a3511`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 0.9 to 2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 0.9 | 0 | 0 | [run](https://argusic.com/run/9aca809d-fb9f-4a2c-91e3-02c0af832a2f) |
| 2 | pass | 100 | 1.5 | 2 | 1 | 1 | [run](https://argusic.com/run/e5c67453-a2d8-45b5-98b1-ddc89bc7da44) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `PEP 668 externally-managed-environment prevented system pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
