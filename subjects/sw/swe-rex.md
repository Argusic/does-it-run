# SWE-ReX

**Verdict: runs.** Argusic Score 83 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SWE-agent/SWE-ReX, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/swe-rex

## Pinned environment

- Project commit: `5c995c365dfb1fd5bc56fda688be5d8538f9931f`
- Test commit: `5c995c365dfb1fd5bc56fda688be5d8538f9931f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7.6 to 23.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 1.5 | 23.1 | 6 | 3 | [run](https://argusic.com/run/0bf6d7d9-b11b-4d8a-a7a0-93a96c76d55f) |
| 2 | pass | 84 | 0.5 | 7.6 | 5 | 1 | [run](https://argusic.com/run/ca823d8e-01a5-443f-b6e3-1ce0d0e9ffe7) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `test_unauthenticated_request: FastAPI's APIKeyHeader returns 401 not 403`
- 1.5 min: `test_bash_multiline_command_eof, test_run_in_shell_interactive_command*: 'python' not found (only python3), 'less' not found`
- 0.5 min: `test_interrupt_pager: 'Killed' output consumed by interrupt handler, not echo`
- `test_docker_deployment*: docker binary not found`
- `test_fargate_deployment*: No AWS region configured`
- `test_modal_deployment*, test_get_modal_deployment: No Modal token`

Attempt 2:

- 1 min: `test_unauthenticated_request expected HTTP 403 but FastAPI returns 401`
- `test_interrupt_pager: less(1) pager not installed in container`
- `Docker tests fail: docker daemon not available in container`
- `Fargate tests fail: AWS credentials not configured`
- `Modal tests fail: MODAL_PROFILE not configured`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
