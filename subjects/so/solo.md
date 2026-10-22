# solo

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/solo-agent/solo, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/solo

## Pinned environment

- Project commit: `9d58e66769ed2479c089b531705f09223d37fff3`
- Test commit: `9d58e66769ed2479c089b531705f09223d37fff3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 55.9 to 55.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 55 | 55.9 | 6 | 4 | [run](https://argusic.com/run/9d0e0a84-488e-4a07-81f2-e83321f9e85a) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Go toolchain and Node 20+ missing from image`
- 15 min: `No Docker/container runtime, but project scripts require docker for PostgreSQL`
- 12 min: `PostgreSQL 16 (jammy build) missing jammy runtime libs libicu70/libldap-2.5-0/libpq5/libreadline8/libtirpc3t64`
- 8 min: `Missing lsof broke make stop/rebuild ('refusing to stop ... not owned by this checkout')`
- 10 min: `message-sharing (headless clipboard), user-avatar (photo upload), channel-split (layout) specs hang in headless Chromium in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
