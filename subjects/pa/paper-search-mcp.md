# paper-search-mcp

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openags/paper-search-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/paper-search-mcp

## Pinned environment

- Project commit: `808e462a824ce6b26fdccbed352b4bf47d7b84cb`
- Test commit: `808e462a824ce6b26fdccbed352b4bf47d7b84cb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 2 | 9.1 | 2 | 0 | [run](https://argusic.com/run/db295d6a-89e9-44a7-9344-46b13f88ef4d) |

## What was observed on a clean machine

Attempt 1:

- `HTTP 429 rate limit on bioRxiv PDF download test (test_biorxiv.py::test_download_and_read)`
- `HTTP 429 rate limit on Semantic Scholar search tests (test_semantic.py: 3 failures)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
