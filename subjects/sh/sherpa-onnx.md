# sherpa-onnx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/k2-fsa/sherpa-onnx, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/sherpa-onnx

## Pinned environment

- Project commit: `040afe360a38e25daaa325ce8889abf93ea02609`
- Test commit: `040afe360a38e25daaa325ce8889abf93ea02609`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.1 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 5.1 | 4 | 4 | [run](https://argusic.com/run/7e58fc4c-3ceb-4899-9ea5-12e4a76f6ad5) |
| 2 | pass | 100 | 7 | 7.2 | 6 | 6 | [run](https://argusic.com/run/d3bc0c81-bbe6-42f7-a0f7-b662d0d812c0) |

## What was observed on a clean machine

Attempt 1:

- 0.4 min: `Missing dependency 'click' when running sherpa-onnx-cli`
- 2.4 min: `Missing dependency 'numpy' and 'soundfile' for audio processing`
- 0.5 min: `Missing dependency 'sentencepiece' for CLI tokenizer`
- 0.4 min: `Missing dependency 'pypinyin' for CLI tokenizer`

Attempt 2:

- `/usr/bin/time was unavailable (exit 127)`
- 3 min: `pip install . failed at CMake configure because Python.h and Development.Module were missing; python3-dev cannot be installed without root`
- 1 min: `Repository tests initially failed with ModuleNotFoundError: _sherpa_onnx`
- 1 min: `A single-process pytest run raised duplicate pybind registration errors`
- 1 min: `pytest mis-collected module-level speaker-test helpers as fixtures`
- `The file utility was unavailable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
