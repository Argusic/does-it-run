# Locals

**Verdict: not yet verified.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Generated-Computers/Locals, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/locals

## Pinned environment

- Project commit: `32cf2feb07cd6e92cde4871347435773393f1812`
- Test commit: `32cf2feb07cd6e92cde4871347435773393f1812`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 20.5 to 20.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 16 | 20.5 | 6 | 6 | [run](https://argusic.com/run/bda37f79-a757-4c82-90dd-afe6d7566b0c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `mlx.core requires libcuda.so.1 (NVIDIA CUDA driver) which is not available on this Linux x86_64 container without a GPU`
- `4 tests fail due to missing CUDA driver (test_oai.py: test_request_temperature, test_a_requests_own_top_p_top_k_and_seed, test_the_one_pass_filters_keep_what_mlx_lms_keep; test_client.py: test_a_prompt_file_that_is_not_utf8_is_named)`
- `5 tests fail due to platform checks in test_app.py - _platform_ok() detects non-Apple OS and sys.exit(1), memory_gb() returns 0 on Linux (no sysctl)`
- `1 test fails in test_connections.py (test_aider_gets_the_base_url_over_the_users_own) - IndexError because _platform_ok() exits before the test logic runs`
- `1 test fails in test_service_idle.py (test_tuning_while_idle_waits_for_the_other_engine) - cannot import locals.kernels which needs mlx.core`
- `26 test files cannot even be collected (15 from importorskip mlx_lm, 11 from direct import mlx.core) - they would need MLX/GPU to run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
