# open-claude-cowork

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/composio-community/open-claude-cowork, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/open-claude-cowork

## Pinned environment

- Project commit: `52335ef50fd033cb5ce87068be0b5b546fa5b73d`
- Test commit: `52335ef50fd033cb5ce87068be0b5b546fa5b73d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 10.1 | 3 | 3 | [run](https://argusic.com/run/7879a769-f97b-421c-b15e-f22b84413133) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Composio SDK throws fatal error when COMPOSIO_API_KEY is unset - crashes server startup`
- 2 min: `Opencode binary not found (spawn opencode ENOENT) - optional provider cannot initialize`
- 1 min: `Electron SUID sandbox helper not configured in container; dbus not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
