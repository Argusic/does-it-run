# redis-vl-python

**Verdict: runs with mocks.** Argusic Score 54 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/redis/redis-vl-python, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/redis-vl-python

## Pinned environment

- Project commit: `8bb2f69e6a6dcd8183eb95e0c02a3b0172da133c`
- Test commit: `8bb2f69e6a6dcd8183eb95e0c02a3b0172da133c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 17.6 to 18.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 17.6 | 0 | 0 | [run](https://argusic.com/run/d1142424-ff1b-4f2e-9eab-161f4bab34d6) |
| 2 | pass with mocks | 88 | 0.5 | 18.8 | 5 | 4 | [run](https://argusic.com/run/2fff3f90-8c9f-4536-b670-588672239ffe) |

## What was observed on a clean machine

Attempt 2:

- 0.2 min: `Missing pydantic-settings dependency for MCP module`
- 0.5 min: `Missing sentence-transformers dependency for HFTextVectorizer`
- 0.3 min: `Missing google-genai dependency for GoogleGenAIVectorizer`
- 0.3 min: `Missing fastmcp dependency for MCP tests`
- `6 CLI unit tests require redis_url fixture (Docker Redis needed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
