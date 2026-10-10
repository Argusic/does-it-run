# AWorld

**Verdict: runs with mocks.** Argusic Score 77 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/inclusionAI/AWorld, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/aworld

## Pinned environment

- Project commit: `631f67f54b68251d71f8a2c5cd5b5ebced2ac6c5`
- Test commit: `631f67f54b68251d71f8a2c5cd5b5ebced2ac6c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 22.7 to 22.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 77 | 17 | 22.7 | 4 | 1 | [run](https://argusic.com/run/495f5134-ecf1-4222-869e-6c5e0eaefe64) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `aworld/cmd/web/api_server.py missing logger import - NameError: name logger is not defined`
- `test_forced_skill_runtime KeyError: llm_base_url - AgentConfig without LLM fails`
- `test_command_bridge tasks command - background_task_manager property checks executor not runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
