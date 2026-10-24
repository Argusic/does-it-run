# AI-company

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CronusL-1141/AI-company, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-company

## Pinned environment

- Project commit: `329c525e5f561df462eee5a89bfdf661adbc2769`
- Test commit: `329c525e5f561df462eee5a89bfdf661adbc2769`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.1 to 44.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 44.1 | 6 | 6 | [run](https://argusic.com/run/76366b79-4ba4-4b84-886d-01cec752b103) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 externally-managed-environment error on 'pip install -e .' in Debian system Python`
- 5 min: `test_restart_development.py::test_source_switch_child_keeps_existing_database fails , subprocess resolves user-site relative to tmp HOME, not finding sqlalchemy installed in /home/runner/.local`
- 2 min: `test_codex_adapter_start.py (2 tests) fail , HTTP MCP preflight fails in isolated HOME; same user-site root cause`
- 2 min: `test_codex_runtime.py (12 tests) fail , subprocesses with isolated HOME can't import psutil from /home/runner/.local`
- 2 min: `test_mcp_concurrency.py, test_mcp_http_sharing.py (4 tests) fail , child process in isolated env can't import psutil`
- 1 min: `test_codex_release_database.py fails , reference commit dd60e97 not present in shallow clone`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
