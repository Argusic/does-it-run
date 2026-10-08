# mysql_mcp_server

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/designcomputer/mysql_mcp_server, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mysql-mcp-server

## Pinned environment

- Project commit: `d88c510f603413d1abad9c5cce2bd542d705e27c`
- Test commit: `d88c510f603413d1abad9c5cce2bd542d705e27c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 7 | 3 | 3 | [run](https://argusic.com/run/f768170f-0f99-4e84-afdd-f65c5dbedd41) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Externally-managed Python environment prevented system-wide pip install`
- 15 min: `MySQL not available in container`
- 3 min: `First mysqld run crashed due to X Plugin socket permission denied and missing secure-file-priv directory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
