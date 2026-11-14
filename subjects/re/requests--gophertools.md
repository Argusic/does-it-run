# requests

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gophertools/requests, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/1757e99f-57fc-406c-ac6c-30b384a7039d

## Pinned environment

- Project commit: `c043f10515bcdc581c88bc6dcbaec3276925b833`
- Test commit: `c043f10515bcdc581c88bc6dcbaec3276925b833`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.3 to 1.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 1.3 | 2 | 2 | [run](https://argusic.com/run/1757e99f-57fc-406c-ac6c-30b384a7039d) |
| 2 | pass | 100 | 1 | 1.5 | 0 | 0 | [run](https://argusic.com/run/4391dc03-2d22-48c5-8aed-ff1ad9c30c2c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go binary not found in PATH; no Go compiler installed in container`
- 1 min: `Permission denied extracting Go tarball to /usr/local (no root access)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
