# nanobot

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HKUDS/nanobot, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/nanobot

## Pinned environment

- Project commit: `d81aa5a4ab420877e43a2a878c26f5635bbef743`
- Test commit: `d81aa5a4ab420877e43a2a878c26f5635bbef743`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 28.4 to 29.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.2 | 28.4 | 0 | 0 | [run](https://argusic.com/run/b105bfe9-e105-42cc-9199-f174872c5c39) |
| 2 | pass with mocks | 92 | 25 | 29.3 | 5 | 5 | [run](https://argusic.com/run/214406aa-0fb8-445b-bcb7-2b88443858ec) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `tests/agent/test_mcp_reconnect_crash.py::test_mcp_reconnect_during_shutdown_does_not_crash failed: mcp 1.30.0's idle-timeout rework left the client session alive, so tool re-execution succeeded without triggering the reconnect the test gate`
- 10 min: `tests/cli/test_commands.py::test_webui_missing_runtime_env_fails_before_starting_gateway and ::test_webui_yes_still_refuses_invalid_custom_model_setup failed under pytest -n 4 because COLUMNS=80 in this container made Rich wrap the config p`
- 5 min: `mock provider 'nanobot agent -m' returned 'Error calling LLM: Connection error.' because the background mock server died when its launching shell exited`
- 5 min: `nanobot TUI: 'no native TUI archive is published for nanobot 0.3.0 on this platform' after uv pip installs replaced the editable install`
- 6 min: `basedpyright reported 1294 errors (unresolved telegram/discord/slack/azure/boto3/langfuse imports) because optional extras and channel deps were not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
