# FreeVideo

**Verdict: runs with mocks.** Argusic Score 66 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FlashML-org/FreeVideo, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/freevideo

## Pinned environment

- Project commit: `500207cb63dc002e74cd268fe39639ae8747d2ef`
- Test commit: `500207cb63dc002e74cd268fe39639ae8747d2ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 3 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 40 | 5.5 | 8.3 | 4 | 2 | [run](https://argusic.com/run/30480d27-316d-4d65-b77f-30a001493292) |
| 2 | pass with mocks | 92 | 10 | 3 | 0 | 0 | [run](https://argusic.com/run/187fbc8a-bd20-4623-8bb1-f561a0f778ad) |

## What was observed on a clean machine

Attempt 1:

- `Hardware detection requires CUDA/NVIDIA GPU: nvidia-smi missing, libcuda.so not found`
- `Web frontend Node.js tests fail: CommonJS modules not importable as ESM named exports with Node 18`
- 1 min: `Externally-managed system Python prevents direct pip install`
- 1.5 min: `Missing PyTorch dependency for hardware detection`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
