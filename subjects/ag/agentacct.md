# agentacct

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mikehasa/agentacct, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agentacct

## Pinned environment

- Project commit: `8c4d3d5eae16fc56916789ad90eb3a690301d71a`
- Test commit: `8c4d3d5eae16fc56916789ad90eb3a690301d71a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 49.6 to 49.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 49.6 | 2 | 2 | [run](https://argusic.com/run/cff15816-7c2f-4077-a56f-a7c407b18ea9) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `container umask 0002 makes test fixture dirs group-writable; production code rejects mode & 0o022`
- 2 min: `_resolve_absolute_mcp_command cannot find absolute agentacct path when venv not on PATH and sys.argv[0] is pytest`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
