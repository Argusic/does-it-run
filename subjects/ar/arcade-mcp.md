# arcade-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ArcadeAI/arcade-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/arcade-mcp

## Pinned environment

- Project commit: `af2501e5640027e07d88dae5ea3cfe92968a88a1`
- Test commit: `af2501e5640027e07d88dae5ea3cfe92968a88a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.4 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 17.4 | 3 | 3 | [run](https://argusic.com/run/f3b077d0-c773-412f-bcf4-24f832ba2352) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `uv binary not installed (make install/health checks require it)`
- 5 min: `arcade whoami exits 1 with 'Not logged in' when no Arcade login config exists (tests/install/test_install.py step 6)`
- 6 min: `arcade show --local finds no tools for the quick-start src-layout scaffold (DISCOVERY_PATTERNS only match top-level *.py and tools/ dirs)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
