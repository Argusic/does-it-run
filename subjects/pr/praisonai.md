# PraisonAI

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MervinPraison/PraisonAI, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/praisonai

## Pinned environment

- Project commit: `5c7d76d72d4ae5ba58365fb8a8a6357185ddc79a`
- Test commit: `5c7d76d72d4ae5ba58365fb8a8a6357185ddc79a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 25.7 to 31.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 31.5 | 5 | 5 | [run](https://argusic.com/run/f697d13f-b28b-48f1-9bde-b9df0ce63721) |
| 2 | pass | 100 | 30 | 25.7 | 5 | 5 | [run](https://argusic.com/run/cc31d33c-ab53-4b7e-b4b0-7ee08b222370) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `test_agent_clone.py expected _current_agent_name_var ContextVar that doesn't exist on LLM`
- 3 min: `current_agent_name was a plain shared attribute on LLM, causing race conditions when concurrent agents shared one LLM instance`
- `praisonai-sandbox not installed - 5 sandbox tests fail with ImportError`
- `TypeScript SDK build fails - @mendable/firecrawl-js dependency missing`
- `Rate limiter retry test fails - resolve_failover_decision retries unknown errors up to 2 times`

Attempt 2:

- 2 min: `Externally-managed Python environment blocked system-wide pip install`
- 3 min: `TS SDK npm build failed due to missing @mendable/firecrawl-js dependency`
- 2 min: `LLM-related tests required litellm (optional dependency)`
- 1 min: `pytest and pytest-asyncio not pre-installed in venv`
- `12 TS test suites failed (40/2659 tests) - pre-existing test mocking issues in UUID crypto and integration/smoke tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
