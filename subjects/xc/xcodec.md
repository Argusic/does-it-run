# xcodec

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhenye234/xcodec, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/xcodec

## Pinned environment

- Project commit: `4a737f2ee2cd061fade92bb2a1a0c78cb8d1eddd`
- Test commit: `4a737f2ee2cd061fade92bb2a1a0c78cb8d1eddd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 8.4 | 3 | 3 | [run](https://argusic.com/run/f8f88c39-a88a-4e42-9b6a-34aa3e617859) |

## What was observed on a clean machine

Attempt 1:

- `scipy==1.10.1 not available for Python 3.12`
- 1 min: `scipy.signal.kaiser moved to scipy.signal.windows in scipy>=1.12`
- 2 min: `torchcodec requires CUDA shared lib not present on CPU torch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
