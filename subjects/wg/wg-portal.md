# wg-portal

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/h44z/wg-portal, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/wg-portal

## Pinned environment

- Project commit: `eb44c8c4ff120f34c26b2415c47560f4fba0603c`
- Test commit: `eb44c8c4ff120f34c26b2415c47560f4fba0603c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.5 to 14.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 14.5 | 5 | 5 | [run](https://argusic.com/run/c67216b2-5ed5-468f-a5ee-1b35f549880b) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `No Go toolchain on system (need >=1.27); Debian package install blocked without root`
- 4 min: `Bundled Node 18.19.1 fails frontend build (vite/rolldown requires node:util styleText)`
- 2 min: `Frontend build required before Go build; go build failed on missing embedded frontend-dist assets`
- 1 min: `Integration-tagged test Test_sqlRepo_migrate panics with nil config (pre-existing, separate from standard suite)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
