# tiny-voca

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/n4ze3m/tiny-voca, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/tiny-voca

## Pinned environment

- Project commit: `62e2adef158bc997042cc6234f541f1e0e4cd55d`
- Test commit: `62e2adef158bc997042cc6234f541f1e0e4cd55d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 5.4 | 3 | 3 | [run](https://argusic.com/run/718d50a8-0d4e-43f0-b4bf-7fab47afafb4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `system Python externally managed (PEP 668) , pip refused to install globally`
- 0.5 min: `dizione phonemizer could not find data (FileNotFoundError)`
- 0.5 min: `ONNX export test failed , module 'onnx' not installed (only onnxruntime was present)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
