# radient

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fzliu/radient, licensed BSD-2-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/radient

## Pinned environment

- Project commit: `89ee872edd6bb2e3b85194c3b85fe1d94b352a0f`
- Test commit: `89ee872edd6bb2e3b85194c3b85fe1d94b352a0f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.8 to 24.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 24.8 | 7 | 7 | [run](https://argusic.com/run/a25ef300-90e7-47b2-a764-bc99edd7e3aa) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `18 modules need from __future__ import annotations to prevent eager LazyImport at class-definition time`
- 2 min: `WhisperSpeechToTextTransform default torch_dtype eagerly evaluates LazyImport`
- 3 min: `SklearnTextVectorizer crashes on single string and missing fit`
- 2 min: `FastRPGraphVectorizer list result crashes metadata attachment`
- 1 min: `RDKitMoleculeVectorizer crashes on invalid SMILES from FDA dataset`
- `DefaultVideoDemuxTransform cannot decode AAC/mp4 via librosa+soundfile`
- `accelerate() fails: torch ONNX exporter incompatible with sentence-transformers BatchEncoding input`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
