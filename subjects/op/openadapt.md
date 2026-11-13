# OpenAdapt

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenAdaptAI/OpenAdapt, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/openadapt

## Pinned environment

- Project commit: `7ae7ebc02048f41dd820ad826d3e78c4dcce2cd2`
- Test commit: `7ae7ebc02048f41dd820ad826d3e78c4dcce2cd2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 20.3 to 63.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 0.25 | 20.3 | 2 | 0 | [run](https://argusic.com/run/fcb5557e-e207-4a6e-95f6-942942892c1d) |
| 2 | pass | 100 | 0.4 | 63.6 | 3 | 3 | [run](https://argusic.com/run/ecc32657-20a7-4ee5-a6f8-25e22122374f) |

## What was observed on a clean machine

Attempt 1:

- `onnxruntime pthread_setaffinity_np spams stderr and causes compile/replay to hang in constrained containers`
- `openadapt flow tutorial hangs during replay phase (onnxruntime OCR thread-spawn issue in this container)`

Attempt 2:

- `onnxruntime pthread_setaffinity_np errors flood stderr during OCR/vision operations`
- `openadapt package has no __main__.py so 'python -m openadapt' fails`
- `break-it tutorial run took ~10 min to complete due to container CPU constraints`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
