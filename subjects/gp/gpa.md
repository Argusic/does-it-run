# GPA

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AutoArk/GPA, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/gpa

## Pinned environment

- Project commit: `3ec1efb402d8598cbaa26e6156cc148a04c60d50`
- Test commit: `3ec1efb402d8598cbaa26e6156cc148a04c60d50`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.3 to 10.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 10.3 | 3 | 3 | [run](https://argusic.com/run/e36229c3-f9a9-4ce4-b498-f545bbf58022) |

## What was observed on a clean machine

Attempt 1:

- `Missing tensor warnings in SparkDeTokenizer (mel_transformer.spectrogram.window, mel_transformer.mel_scale.fb)`
- `CPU autocast dtype warning in spark_tokenizer.py and spark_detokenizer.py`
- `Failed to load CPU gemm_4bit_forward from kernels-community`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
