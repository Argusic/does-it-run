# GPT-SoVITS

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RVC-Boss/GPT-SoVITS, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gpt-sovits

## Pinned environment

- Project commit: `48b1a0169a28582a8984402f82cf438d3bfa6aca`
- Test commit: `48b1a0169a28582a8984402f82cf438d3bfa6aca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.9 to 22.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 22.9 | 4 | 4 | [run](https://argusic.com/run/20806a30-7a61-477b-b805-9b533c992d91) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `opencc build from source failed (missing C dependencies)`
- 8 min: `pyopenjtalk failed - Python.h not found`
- 3 min: `jieba_fast failed - Python.h not found`
- 1 min: `NLTK averaged_perceptron_tagger_eng missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
