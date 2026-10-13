# auto-browser

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LvcidPsyche/auto-browser, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/auto-browser

## Pinned environment

- Project commit: `6b2c196bb517454603c01370961326a08cd8bcb5`
- Test commit: `6b2c196bb517454603c01370961326a08cd8bcb5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.7 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 5.7 | 1 | 1 | [run](https://argusic.com/run/e5e3545d-a7ef-4040-8f53-bf90d06d0f67) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `OPENROUTER_API_KEY env var in container leaks into pydantic-settings, causing test_not_configured_without_api_key to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
