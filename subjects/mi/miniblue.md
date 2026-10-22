# miniblue

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/moabukar/miniblue, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/miniblue

## Pinned environment

- Project commit: `22b04dbbf4f3d1257898eed5ad9eb55529302324`
- Test commit: `22b04dbbf4f3d1257898eed5ad9eb55529302324`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.6 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 6 | 9.6 | 3 | 2 | [run](https://argusic.com/run/ec12e26a-8c50-4aea-bbdb-cb96c4e7381b) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Go (golang) 1.26 not installed on system`
- 1 min: `Go std library src tree had missing go.mod/go.sum (copied from pkg/share instead of pkg/lib)`
- `Integration tests fail: Docker not available for MySQL containers (rootless Docker not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
