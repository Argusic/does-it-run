# datacat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/replit/datacat, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/datacat

## Pinned environment

- Project commit: `f08fb635fd7f28f6ed725209382af3e2c2673676`
- Test commit: `f08fb635fd7f28f6ed725209382af3e2c2673676`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.9 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 5.5 | 4 | 4 | [run](https://argusic.com/run/41cffa83-7440-4c5a-80b8-4e01f19c839e) |
| 2 | pass | 100 | 10 | 3.9 | 0 | 0 | [run](https://argusic.com/run/4d67b855-5701-47d4-bec6-cb30745d7d02) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 does not meet the >=22.15.0 requirement`
- `corepack not found with system node`
- 3 min: `PostgreSQL not installed (no root)`
- 1 min: `PostgreSQL could not create /var/run/postgresql lock file (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
