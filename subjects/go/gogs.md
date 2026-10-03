# gogs

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gogs/gogs, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gogs

## Pinned environment

- Project commit: `aec2b842cdb6b601ef2ed27d20fa78a37ca4a0ea`
- Test commit: `aec2b842cdb6b601ef2ed27d20fa78a37ca4a0ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 14.9 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/97c3c3c3-3284-4f33-9fcf-cc3d04815ee8) |
| 2 | pass | 100 | 27 | 30.9 | 6 | 6 | [run](https://argusic.com/run/f3672161-f35c-4954-bb63-68b07c837f22) |
| 3 | pass | 80 | 30 | 14.9 | 1 | 0 | [run](https://argusic.com/run/1cb88be3-e600-46e4-bb4d-f91da0d4b3f5) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Go compiler not installed`
- 2 min: `Node.js v18 too old for pnpm@11`
- 1 min: `moonrepo CLI not installed`
- 2 min: `ssh-keygen not found (openssh-client not installed)`
- 2 min: `RUN_USER mismatch prevented server start (default 'git', actual 'runner')`
- 5 min: `Dev mode server failed with 502 due to missing Vite proxy on port 5173`

Attempt 3:

- `TestSSHParsePublicKey requires ssh-keygen (openssh-client) which is not installed and cannot be installed without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
