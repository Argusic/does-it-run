# obsidian-wiki

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Ar9av/obsidian-wiki, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/obsidian-wiki

## Pinned environment

- Project commit: `2f10142991344fe9526762e6f296594844c8477b`
- Test commit: `2f10142991344fe9526762e6f296594844c8477b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7.2 | 4.3 | 2 | 2 | [run](https://argusic.com/run/0e3c01a5-b3bf-467c-a989-73377bfc96af) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `pip install failed: externally-managed-environment (PEP 668)`
- 0.2 min: `test_sync.py::test_does_not_reinit_existing_repo failed: git commit returned exit 128 (no user config)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
