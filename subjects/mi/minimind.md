# minimind

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jingyaogong/minimind, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/minimind

## Pinned environment

- Project commit: `f659b55761b754d306bd140573493a6543cafd7f`
- Test commit: `f659b55761b754d306bd140573493a6543cafd7f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12 to 12 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 12 | 2 | 2 | [run](https://argusic.com/run/3671ba3f-914b-4447-99b9-6aab7c72bcf0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Python is externally managed (PEP 668); pip install to system Python fails`
- 2 min: `ujson==5.1.0 failed to build from source: missing Python.h (no python3-dev headers); no root to install system packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
