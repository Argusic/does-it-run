# SuggestArr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/giuseppe99barchetta/SuggestArr, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/suggestarr

## Pinned environment

- Project commit: `809353da4dc1ade2c5deeb421c2103f8ed2dbfa7`
- Test commit: `809353da4dc1ade2c5deeb421c2103f8ed2dbfa7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.8 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 2.8 | 0 | 0 | [run](https://argusic.com/run/77ee2062-acd2-4a06-a6e0-1c47d885aa6d) |
| 2 | pass | 100 | 14 | 4.2 | 1 | 1 | [run](https://argusic.com/run/3d91c49f-6b48-4281-bf6d-754415aa2d6f) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `PEP 668 externally-managed environment blocks system-wide pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
