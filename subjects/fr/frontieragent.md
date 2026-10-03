# FrontierAgent

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ApodexAI/FrontierAgent, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/frontieragent

## Pinned environment

- Project commit: `a3c1be339c249ead2a16f3f4c9a1e7c21059e8fc`
- Test commit: `a3c1be339c249ead2a16f3f4c9a1e7c21059e8fc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 39.9 to 39.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.1 | 39.9 | 4 | 4 | [run](https://argusic.com/run/5539c023-1991-4d83-8ae6-8072f0e0dc69) |

## What was observed on a clean machine

Attempt 1:

- 0.02 min: `uv not in PATH at start`
- `TUI tests (apodex/tests/test_tui.py, 170 tests) need a real Textual terminal`
- `test_a_slow_endpoint_fails has an intentional 90s mock-server delay, hangs outside its 120s timeout on single run`
- 10 min: `CLI --print mode failed to reach a standalone mock server due to asyncio httpx IPv6 resolution order and background process lifecycle in this shell; the project's own in-process MockLLMServer (used in test_hf_space_runtime.py) works correct`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
