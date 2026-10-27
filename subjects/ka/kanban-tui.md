# kanban-tui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Zaloog/kanban-tui, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/kanban-tui

## Pinned environment

- Project commit: `1f96443e3ba67b398939996823442b19ea60fe61`
- Test commit: `1f96443e3ba67b398939996823442b19ea60fe61`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 5 | 2 | 2 | [run](https://argusic.com/run/3a97f564-ee5b-4c66-a560-5840c3762c4a) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `uv not installed in container; system pip blocked by PEP 668 externally-managed-environment`
- 5 min: `14 test failures + 2 collection errors: ModuleNotFoundError atlassian (jira extra not in dev group), skills/mcp command test failures (pycli-mcp missing), test_config.py import errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
