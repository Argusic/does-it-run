# rag-api

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LibreChat-AI/rag-api, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/rag-api

## Pinned environment

- Project commit: `c4e5cbf79fcece1df9adfff5dfed983a5990ca9f`
- Test commit: `c4e5cbf79fcece1df9adfff5dfed983a5990ca9f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 4.2 | 2 | 2 | [run](https://argusic.com/run/e4fd1d0c-87b4-4630-89a4-e17fc450ea57) |

## What was observed on a clean machine

Attempt 1:

- `pandoc not installed (6 tests skipped in test_lazy_load.py)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
