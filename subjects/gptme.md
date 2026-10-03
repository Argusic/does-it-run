# gptme

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gptme/gptme, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gptme

## Pinned environment

- Project commit: `f26d7dbe57d855dd6de68d8b0bfb44e09227087e`
- Test commit: `f26d7dbe57d855dd6de68d8b0bfb44e09227087e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34.3 to 34.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 34.3 | 3 | 3 | [run](https://argusic.com/run/c30557c7-7054-46de-a19c-8fb996573730) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_agent.py::TestCLI::test_install_detects_existing_workspace failed because 'get_service_manager()' returns None in this environment (no systemd/launchd) but the test didn't mock it`
- 15 min: `test_native_ipython_highlight_preserves_literal_source failed because 'rich_to_str()' creates a Console that inherits NO_COLOR=1 and TERM=dumb from the environment, suppressing ANSI output even with force_terminal=True`
- 10 min: `test suite hung when running with many test files due to leftover shell processes from test_tools_shell.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
