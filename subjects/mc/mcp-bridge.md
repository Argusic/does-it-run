# MCP-Bridge

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SecretiveShell/MCP-Bridge, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-bridge

## Pinned environment

- Project commit: `df1dcc58cac7bf2a4ead5f5630eb970f42999c57`
- Test commit: `df1dcc58cac7bf2a4ead5f5630eb970f42999c57`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 3.5 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 6.4 | 1 | 1 | [run](https://argusic.com/run/d1afe3a2-162b-4490-80bb-6249f13ed4da) |
| 2 | fail | 80 | 0.5 | 3.5 | 1 | 1 | [run](https://argusic.com/run/8123c8a9-fdd8-49cc-8991-ddc3c163cb88) |

## What was observed on a clean machine

Attempt 1:

- `pydantic field name 'json' shadows parent attribute in InitialSettings`

Attempt 2:

- 0.1 min: `Field name 'json' in 'InitialSettings' shadows an attribute in parent 'BaseSettings' - pydantic warning`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
