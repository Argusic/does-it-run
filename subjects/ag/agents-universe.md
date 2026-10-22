# agents-universe

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agents-universe/agents-universe, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agents-universe

## Pinned environment

- Project commit: `c73e89e7bff73e073def5adfa9eb61fdadfa6762`
- Test commit: `c73e89e7bff73e073def5adfa9eb61fdadfa6762`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 36.6 to 36.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 55 | 36.6 | 3 | 3 | [run](https://argusic.com/run/57845659-6dff-4f84-9779-a8f490ddfeef) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `agent-core pytest: 7 sandbox/shell tests failed (1642 passed) - sandbox guard sitecustomize user-site channel unavailable in venv (ENABLE_USER_SITE False), no python on PATH (only python3), venv-editable agent_core path not a guard read roo`
- 20 min: `uvicorn --env-file not honored for settings - server started with default MSSQL URL (libodbc missing, /api/projects/{id}/knowledge 404; /api/projects by slug 404)`
- 10 min: `model-config test-connection rejects loopback base_url (SSRF literal-IP block) and mock returns non-SSE to stream`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
