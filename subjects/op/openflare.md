# OpenFlare

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Rain-kl/OpenFlare, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/openflare

## Pinned environment

- Project commit: `c3606bc6f6f0df5c4143f618db8e8c4536b1bad4`
- Test commit: `c3606bc6f6f0df5c4143f618db8e8c4536b1bad4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.4 to 20.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 20.4 | 6 | 6 | [run](https://argusic.com/run/a1f1aed4-bad9-4027-ad81-c479320452df) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25.x not in PATH`
- 1 min: `Node 18 shipped no longer supports corepack-shim downloads`
- 1 min: `pnpm not available after corepack failed`
- 3 min: `Redis not installed`
- `PostgreSQL not available in container`
- 2 min: `Server died after background launch due to process-group cleanup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
