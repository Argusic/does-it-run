# automem

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/verygoodplugins/automem, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/automem

## Pinned environment

- Project commit: `0e8c4174b799abb9eab3370400a80ea9e8ad1f02`
- Test commit: `0e8c4174b799abb9eab3370400a80ea9e8ad1f02`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 15 to 22 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 15 | 2 | 2 | [run](https://argusic.com/run/37a5633d-b225-436e-acc7-4c5e5b83f019) |
| 2 | fail | 20 | n/a | 22 | 0 | 0 | [run](https://argusic.com/run/098793cf-d0a2-4470-a9da-0191b0725b2c) |

## What was observed on a clean machine

Attempt 1:

- `docker compose/services unavailable in container (no docker binary)`
- `model download for embeddings missing (no network during app init); onnx runtime OK via cached model`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
