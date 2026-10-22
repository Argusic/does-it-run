# python-utcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/universal-tool-calling-protocol/python-utcp, licensed MPL-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/python-utcp

## Pinned environment

- Project commit: `3730c46633333b1527c56aae7f33d53800eda1f1`
- Test commit: `3730c46633333b1527c56aae7f33d53800eda1f1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.8 to 20.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 20.8 | 2 | 2 | [run](https://argusic.com/run/9d50f58f-afcb-4c85-83c8-935a923fd168) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Externally-managed Python environment prevents system-wide pip install`
- 1 min: `Missing numpy dependency blocks in_mem_embeddings plugin test collection`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
