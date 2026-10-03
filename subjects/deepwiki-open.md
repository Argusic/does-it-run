# deepwiki-open

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AsyncFuncAI/deepwiki-open, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/deepwiki-open

## Pinned environment

- Project commit: `d92819a9c9f3b99416e3580ff235fc9d3adf8b89`
- Test commit: `d92819a9c9f3b99416e3580ff235fc9d3adf8b89`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 21.1 to 21.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 24 | 21.4 | 3 | 3 | [run](https://argusic.com/run/f3e9b5f4-9c00-472f-8f21-f41ed7d69d94) |
| 2 | pass | 100 | 19 | 21.3 | 10 | 10 | [run](https://argusic.com/run/27302a66-fd88-4e3a-98bd-9b2cfc8ae634) |
| 3 | pass with mocks | 92 | 20.9 | 21.1 | 3 | 3 | [run](https://argusic.com/run/4aee03e8-4e22-466e-867d-fc2e75eb8e52) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Poetry not installed`
- 1 min: `pytest-mock not in dev dependencies`
- `3 tests require real GOOGLE_API_KEY or OPENAI_API_KEY (embedder API calls)`

Attempt 2:

- 2 min: `Missing uv and root pyproject.toml - uv.lock existed but no project file`
- 1 min: `Missing gitpython package`
- 1 min: `Missing watchfiles package`
- 1 min: `Missing websockets package`
- 1 min: `Missing pytest-asyncio for async tests`
- 1 min: `Missing pytest-mock for mocker fixture`
- 5 min: `Frontend build OOM killed during next build static generation (1GB RAM limit)`
- 2 min: `Stale test files import removed modules (api.google_embedder_client, api.tools.embedder)`
- 1 min: `3 integration tests use return True/False instead of assert, confusing pytest`

Attempt 3:

- 1 min: `pyproject.toml in api/ used Poetry format (package-mode=false) incompatible with uv sync`
- 0.5 min: `Missing pytest-mock dependency , tests/test_repository.py uses mocker fixture`
- 0.3 min: `uv not available on PATH (installed via pip but not in PATH)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
