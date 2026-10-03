# oomwoo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/makerspet/oomwoo, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/oomwoo

## Pinned environment

- Project commit: `840d9c37639172408fd2ffaa7babaadf814a1032`
- Test commit: `840d9c37639172408fd2ffaa7babaadf814a1032`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.5 to 2.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.1 | 2.5 | 1 | 1 | [run](https://argusic.com/run/ee3ab72d-33c7-4434-961b-e9458f02f31e) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `pytest not available (PEP 668 blocks system pip)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
