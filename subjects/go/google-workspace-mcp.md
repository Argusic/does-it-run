# google_workspace_mcp

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/taylorwilsdon/google_workspace_mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/google-workspace-mcp

## Pinned environment

- Project commit: `ed70fb9068231ee13484bc2d53bdde2451e34d31`
- Test commit: `ed70fb9068231ee13484bc2d53bdde2451e34d31`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 30.8 to 30.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 2 | 30.8 | 1 | 0 | [run](https://argusic.com/run/15676ab7-82a8-4653-a25d-ada5d944ff82) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `25 tests in test_contacts_integration.py fail when run after other test files due to shared module-level state (pass 242/242 in isolation)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
