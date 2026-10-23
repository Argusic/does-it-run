# onnx-asr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/istupakov/onnx-asr, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/onnx-asr

## Pinned environment

- Project commit: `675f0e68c24d846ee1775743e92d9b4ed452380e`
- Test commit: `675f0e68c24d846ee1775743e92d9b4ed452380e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.2 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 12.2 | 2 | 2 | [run](https://argusic.com/run/cd51f163-935b-4fb3-a7fc-b04cd450564f) |

## What was observed on a clean machine

Attempt 1:

- `6 preprocessors tests skipped: missing torch, onnx, kaldi_native_fbank (test-all deps, not core)`
- `onnxruntime pthread_setaffinity_np warnings in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
