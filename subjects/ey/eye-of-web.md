# eye_of_web

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MehmetYukselSekeroglu/eye_of_web, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/eye-of-web

## Pinned environment

- Project commit: `943644f5b6e9ab3a4fd7a10d1ee3ba051fdadd19`
- Test commit: `943644f5b6e9ab3a4fd7a10d1ee3ba051fdadd19`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 11.7 | 3 | 3 | [run](https://argusic.com/run/ea53e8ef-a41a-4dde-aa3c-ee224366970c) |

## What was observed on a clean machine

Attempt 1:

- `tgcrypto package failed to build (missing python3-dev / Python.h)`
- `Torch/TorchVision not installed from requirements due to package being excluded for image size`
- 2 min: `PostgreSQL and Milvus services unavailable in container; mock files created at src/mocks/db_mock.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
