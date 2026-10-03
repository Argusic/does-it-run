# sentrysearch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ssrajadh/sentrysearch, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/sentrysearch

## Pinned environment

- Project commit: `316a171e880b674ec1718e7d224d0b2fb8fb10a5`
- Test commit: `316a171e880b674ec1718e7d224d0b2fb8fb10a5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.3 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 9.3 | 1 | 1 | [run](https://argusic.com/run/f0dea3e7-3214-4eff-9f21-8e7d124b664b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Local Qwen3-VL-Embedding-2B model OOM-killed during weight loading (cgroup memory limit 8GB, container has no GPU)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
