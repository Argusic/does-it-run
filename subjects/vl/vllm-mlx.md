# vllm-mlx

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/waybarrios/vllm-mlx, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/vllm-mlx

## Pinned environment

- Project commit: `37a16c76bb21c3bd94350db1e48ed71220aaa5d4`
- Test commit: `37a16c76bb21c3bd94350db1e48ed71220aaa5d4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 23.4 to 23.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 23.4 | 1 | 1 | [run](https://argusic.com/run/c78577a7-1f77-4146-915a-d207194c5d93) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `4 Apple-Silicon-only test scripts (test_paged_cache_benefits.py, test_paged_cache_real_inference.py, test_paged_cache_real_model.py, test_registry_idle_unload_real_model.py) called sys.exit(0) at module level on non-Apple-Silicon platforms,`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
