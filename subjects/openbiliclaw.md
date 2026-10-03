# OpenBiliClaw

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/whiteguo233/OpenBiliClaw, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/openbiliclaw

## Pinned environment

- Project commit: `3c53294e7679f9947498e584f60e941dc8aa8211`
- Test commit: `3c53294e7679f9947498e584f60e941dc8aa8211`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 4; wall time 42 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/9896baab-7f50-42a9-a130-caf9cff4d6ab) |
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/601ebf0a-3053-4b4e-8cfa-d5cd5b2e50d1) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/66ba8463-87a5-4052-b2a7-70b01a014497) |
| 2 | pass with mocks | 92 | 8 | 76.3 | 3 | 3 | [run](https://argusic.com/run/7123175a-f2a1-4f52-9d9d-a764e2c8d8fd) |

## What was observed on a clean machine

Attempt 2:

- `test_api_app.py::TestBackendAPI::test_runtime_status_endpoint_returns_runtime_summary - install_mode='docker' vs expected 'unsupported' due to /.dockerenv detection`
- `test_api_degraded_mode.py::test_degraded_init_status_reports_degraded_reason - unsupported_runtime vs expected degraded due to old config format in test fixture`
- 5 min: `test_api_weibo.py::test_weibo_share_count_survives_recommendation_and_delight_http_serialization - FakeDatabase.get_delight_candidates missing include_delivered parameter`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
