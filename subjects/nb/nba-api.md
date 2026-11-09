# nba_api

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/swar/nba_api, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/nba-api

## Pinned environment

- Project commit: `52c0fb0b81c4b785d6cebeb9988799e5d796dfd7`
- Test commit: `52c0fb0b81c4b785d6cebeb9988799e5d796dfd7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 12.6 to 38.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 32 | 38.5 | 0 | 0 | [run](https://argusic.com/run/223c237b-c358-4e58-ad05-154f2cff80d5) |
| 2 | pass with mocks | 92 | 0.5 | 12.6 | 2 | 2 | [run](https://argusic.com/run/1d942759-d7a3-4e08-b1a5-e536d1ff59b6) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `VCR cassettes recorded with season 2025-26 fail to match when current date generates season 2026-27 (Nov 2026)`
- 20 min: `test_endpoint_uses_global_session fails when run after VCR integration tests in same pytest session (pre-existing test isolation bug)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
