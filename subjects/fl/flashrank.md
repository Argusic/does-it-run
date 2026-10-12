# FlashRank

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PrithivirajDamodaran/FlashRank, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/flashrank

## Pinned environment

- Project commit: `11f7a40d625f2de047c371c81c6f477386c18bb1`
- Test commit: `11f7a40d625f2de047c371c81c6f477386c18bb1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.7 to 1.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 1.7 | 3 | 3 | [run](https://argusic.com/run/13ef3d5c-fe6e-4b57-ae4e-ca7310007504) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install refused because system Python 3.12 is externally managed (PEP 668, externally-managed-environment)`
- 3 min: `onnxruntime 1.31.0 repeatedly logs 'pthread_setaffinity_np failed ... error code: 22 Invalid argument' in this container during session creation`
- 1 min: `The library downloads its reranker model from HuggingFace (prithivida/flashrank) at first use; a motivated user must be online to fetch the ~4.8MB zip`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
