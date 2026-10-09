# Aegis

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GanyuanRan/Aegis, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/aegis

## Pinned environment

- Project commit: `0787002a06f0df434befa2e34a629adf20131f3b`
- Test commit: `0787002a06f0df434befa2e34a629adf20131f3b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.8 to 14.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 14.8 | 1 | 1 | [run](https://argusic.com/run/1295107e-e5d3-4646-b1b6-9369298f46f6) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `bwrap "permission-profile backend bwrap is unavailable" prevents agentic-benchmark dry-run profile checks`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
