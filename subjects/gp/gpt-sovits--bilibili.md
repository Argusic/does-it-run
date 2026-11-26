# GPT-SoVITS

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bilibili/GPT-SoVITS, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/ebe49aed-97b3-408c-b1e3-df299f6aac75

## Pinned environment

- Project commit: `6d51ffceafbf240145619af4c92408a6e54b7924`
- Test commit: `6d51ffceafbf240145619af4c92408a6e54b7924`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 14.1 to 30.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 30.8 | 2 | 2 | [run](https://argusic.com/run/ebe49aed-97b3-408c-b1e3-df299f6aac75) |
| 2 | pass | 100 | 29 | 14.1 | 8 | 8 | [run](https://argusic.com/run/270b4841-79c8-4a5b-ad1a-d7db6fc9ef35) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `pyopenjtalk>=0.4.1 failed to build from source: missing python3.12-dev headers (Python.h not found) and cmake 4.x from pip build env broke the project's old CMakeLists.txt`
- 1 min: `pip install refused in system Python due to PEP 668 externally-managed-environment detection`

Attempt 2:

- 5 min: `Missing Python.h - python3.12-dev headers not installed (no root access to apt)`
- 2 min: `jieba_fast failed to build (needs Python.h and pyconfig.h)`
- 4 min: `pyopenjtalk failed to build (missing Python.h and also openjtalk.cpp source path issue)`
- 1 min: `numpy<2.0 requirement conflicts with scipy 1.18 and numba 0.68 which need numpy>=2`
- 2 min: `huggingface-hub version conflict: transformers >=4.51 needs huggingface-hub>=0.34 but gradio 4.44.1 needs HfFolder (removed in 0.26+)`
- 1 min: `opencc C extension failed to build`
- 1 min: `No wget or unzip binary for model downloads`
- 1 min: `No conda available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
