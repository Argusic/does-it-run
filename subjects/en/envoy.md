# Envoy

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/regrevia/Envoy, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/envoy

## Pinned environment

- Project commit: `9428dc508b96e4510f90d051480f680f2af4dfef`
- Test commit: `9428dc508b96e4510f90d051480f680f2af4dfef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.7 to 23.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 2 | 23.7 | 12 | 6 | [run](https://argusic.com/run/f4c75e2f-319b-48ec-a127-9b0e3189b77d) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Missing reportlab for PDF test fixtures`
- 1 min: `Missing backend deps (fastapi, celery, etc) for API tests`
- 0.2 min: `Missing pip in .venv`
- 0.3 min: `test_runtime_safety: mock multiprocessing SimpleNamespace missing current_process`
- 0.3 min: `test_runtime_safety: whisper mock load_model lambda did not accept **kwargs`
- 0.3 min: `test_long_task: network_error now maps to BLOCKED not FAILED`
- `test_browser_runtime: 11 tests fail - Chromium browser not installed (~683 MB)`
- `test_runtime_safety: Tesseract OCR not available (no root for apt install)`
- `test_delivery_package_validator: large video test reports missing_python_media_dependency`
- `test_windows_acceptance_workflow: 2 failures (runner labels, dispatch condition)`
- `test_envoy_cli_distribution: wheel build test hangs`
- `test_install_script: SHA256SUMS mismatch in offline version test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
