# FossFLOW

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Abrar74774/FossFLOW, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/fossflow

## Pinned environment

- Project commit: `0cccb06abdb73b5c30a74e9827d928842b190824`
- Test commit: `0cccb06abdb73b5c30a74e9827d928842b190824`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.3 to 18.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 18.3 | 3 | 3 | [run](https://argusic.com/run/fbe52773-621e-47d3-ae73-373dc12f8671) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js version 18 < required >=24`
- 1 min: `test-diagram.json missing from e2e test copy path`
- 1 min: `test_node_placement.py driver fixture used webdriver.Remote instead of Chrome`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
