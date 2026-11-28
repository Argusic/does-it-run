# HAIR

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DAB-LABS/HAIR, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/hair

## Pinned environment

- Project commit: `69335b0ae5b355e19141b67e00e671e3686f2c6c`
- Test commit: `69335b0ae5b355e19141b67e00e671e3686f2c6c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.4 to 24.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 24.4 | 1 | 1 | [run](https://argusic.com/run/91becadf-0ab5-464f-8742-412f08bd2265) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Python 3.13 was required but only 3.12 was available in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
