# robusta

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/robusta-dev/robusta, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/robusta

## Pinned environment

- Project commit: `1207e8e2c34f853f807c75a3139ae94ebae3f2bb`
- Test commit: `1207e8e2c34f853f807c75a3139ae94ebae3f2bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 1.1 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4.5 | 12.4 | 4 | 4 | [run](https://argusic.com/run/c5edcd70-46cb-4041-864d-432c69b69eaf) |
| 2 | fail | 20 | n/a | 1.1 | 0 | 0 | [run](https://argusic.com/run/e1f687f4-e008-4552-bb08-ae856e895f4d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python version constraint too strict: pyproject.toml required >=3.10, <3.12 but only Python 3.12 is available in container`
- 0.5 min: `Missing dependency 'strenum' not listed in pyproject.toml, causing ModuleNotFoundError on import`
- 0.5 min: `get_all_namespace_data() in api_client_utils.py only caught ApiException but connection refused errors from urllib3 are not ApiException, causing test failures (17 scope_matching tests) and crash when no Kubernetes cluster is present`
- 0.5 min: `test_discovery_recovery_on_failure only patched kubernetes.client.CoreV1Api.list_node but discovery_process calls AppsV1Api.list_deployment_for_all_namespaces first, hitting real connection error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
