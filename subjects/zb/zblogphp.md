# zblogphp

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zblogcn/zblogphp, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/zblogphp

## Pinned environment

- Project commit: `af674c47b6778d8fbacb4a18e9514936631e06b6`
- Test commit: `af674c47b6778d8fbacb4a18e9514936631e06b6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 8.6 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 8.6 | 0 | 0 | [run](https://argusic.com/run/15a03976-54c9-4502-8f98-ee24c85d15b3) |
| 2 | pass | 100 | 9 | 9.3 | 3 | 3 | [run](https://argusic.com/run/7150635e-f70a-4c99-ad6e-1cb92ad5f40c) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `PHP binary not found in container (no root for apt).`
- 0.5 min: `Composer not found.`
- 1 min: `Initial CLI install failed with 'Unable to open database file' when absolute /tmp/zblog.db was passed , code prepends datadir path.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
