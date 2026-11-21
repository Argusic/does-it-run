# auto-browser

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LvcidPsyche/auto-browser, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/auto-browser

## Pinned environment

- Project commit: `6b2c196bb517454603c01370961326a08cd8bcb5`
- Test commit: `6b2c196bb517454603c01370961326a08cd8bcb5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 5.7 | 1 | 1 | [run](https://argusic.com/run/e5e3545d-a7ef-4040-8f53-bf90d06d0f67) |
| 2 | pass | 100 | 2 | 9.7 | 2 | 2 | [run](https://argusic.com/run/0c15911c-f800-47b9-9e86-07abdd7bd961) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `OPENROUTER_API_KEY env var in container leaks into pydantic-settings, causing test_not_configured_without_api_key to fail`

Attempt 2:

- 3 min: `Test test_not_configured_without_api_key failed because the container had OPENROUTER_API_KEY env var set, which pydantic-settings picks up from os.environ, making the adapter report as configured`
- 1 min: `Non-critical: harness extension init failed , /data directory not writable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
