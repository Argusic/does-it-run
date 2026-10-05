# TradingAgents-astock

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/simonlin1212/TradingAgents-astock, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/tradingagents-astock

## Pinned environment

- Project commit: `b0594a4f2b8ff7c32807ebc9ec269007fffe895c`
- Test commit: `b0594a4f2b8ff7c32807ebc9ec269007fffe895c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.6 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 12.6 | 3 | 3 | [run](https://argusic.com/run/6cfc7ee4-114e-4e76-94ab-491cad36943e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install failed due to externally-managed-environment (PEP 668) , system Python blocks global pip install`
- 1 min: `pytest not installed in the venv`
- 15 min: `3 test_streaming_keeps_usage_stats tests failed due to test pollution: test_cli_default_command.py imports cli.main which calls load_dotenv() at module level, reading .env (from .env.example) and setting API keys to empty strings. conftest`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
