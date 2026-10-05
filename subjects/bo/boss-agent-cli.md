# boss-agent-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/can4hou6joeng4/boss-agent-cli, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/boss-agent-cli

## Pinned environment

- Project commit: `cf38175d11a100a8a9e906d272dac716b8f9c934`
- Test commit: `cf38175d11a100a8a9e906d272dac716b8f9c934`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.7 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 13.7 | 2 | 2 | [run](https://argusic.com/run/43334411-3306-4399-ac6a-2243cf4d53cb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Fresh environment had no uv; 'pip install uv' then 'uv sync --all-extras' installed all deps cleanly, but the plain README flow ran into an unrelated missing-dependency problem at the installed entry point: 'boss-mcp --help' failed with 'Mo`
- 1 min: `Patchright chromium was missing, so 'doctor' warned and browser-channel commands fail.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
