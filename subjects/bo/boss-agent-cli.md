# boss-agent-cli

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/can4hou6joeng4/boss-agent-cli, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/boss-agent-cli

## Pinned environment

- Project commit: `cf38175d11a100a8a9e906d272dac716b8f9c934`
- Test commit: `cf38175d11a100a8a9e906d272dac716b8f9c934`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 13.4 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 13.7 | 2 | 2 | [run](https://argusic.com/run/43334411-3306-4399-ac6a-2243cf4d53cb) |
| 2 | pass | 100 | 10 | 13.4 | 1 | 1 | [run](https://argusic.com/run/bad71195-566d-46dc-9c22-148c67449582) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Fresh environment had no uv; 'pip install uv' then 'uv sync --all-extras' installed all deps cleanly, but the plain README flow ran into an unrelated missing-dependency problem at the installed entry point: 'boss-mcp --help' failed with 'Mo`
- 1 min: `Patchright chromium was missing, so 'doctor' warned and browser-channel commands fail.`

Attempt 2:

- `Flaky PTY test test_prompt_toolkit_pty_uses_stderr_and_arrow_keys fails in container: wizard rendered and responded to arrow key selection + Enter, printing exit message, but process.poll() returned None within the 20s PTY_EXIT_TIMEOUT`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
