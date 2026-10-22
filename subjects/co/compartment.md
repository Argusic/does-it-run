# Compartment

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MaxFreedomPollard/Compartment, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/compartment

## Pinned environment

- Project commit: `05c2816a730b9f69aee4344008cfed07dcb88fd8`
- Test commit: `05c2816a730b9f69aee4344008cfed07dcb88fd8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 75.8 to 75.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 75.8 | 3 | 3 | [run](https://argusic.com/run/b753f350-6b9b-41db-9f2b-1f3f07a75c81) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `python3 externally-managed-environment blocks system-wide pip install`
- 2 min: `test_seed_relevance_regression: max_ms 1800+ exceeded 500ms bound from cold ONNX model load`
- 1 min: `test_index_parity_brute_vs_hnsw: ModuleNotFoundError for usearch (optional [hnsw] extra)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
