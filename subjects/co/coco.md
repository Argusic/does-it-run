# coco

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coco-research/coco, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/coco

## Pinned environment

- Project commit: `309d58d175bc9fdce53fef28895dccef199f8b6e`
- Test commit: `309d58d175bc9fdce53fef28895dccef199f8b6e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.5 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 5.5 | 1 | 1 | [run](https://argusic.com/run/7b8f74f0-b182-4be9-88a1-62c6d3d6830e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing Python module pyyaml`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
