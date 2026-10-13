# unifi-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sirkirby/unifi-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/unifi-mcp

## Pinned environment

- Project commit: `466c2f2a538ae25eec408b01be7d5e0c972aff6e`
- Test commit: `466c2f2a538ae25eec408b01be7d5e0c972aff6e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18.2 to 18.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 26 | 18.2 | 5 | 5 | [run](https://argusic.com/run/33f5d4f5-b797-4c58-9b68-dd13554cd7da) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No uv and no Python 3.13 in container`
- 6 min: `Detached HEAD at untagged commit: test_version_matches_git_tag failed (importlib version 0.0.1.dev1+g466c2f2a5 vs git describe bare hash 466c2f2)`
- 5 min: `Worker prerequisite test failed: Node 18 < required 22`
- 2 min: `After checkout change, uv env had no ruff/tests`
- 3 min: `API server failed startup on fresh DB (no such table: controllers)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
