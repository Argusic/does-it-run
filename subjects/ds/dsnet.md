# dsnet

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/naggie/dsnet, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/dsnet

## Pinned environment

- Project commit: `d5eca4e18b934134985674e3227416ba1d89c36f`
- Test commit: `d5eca4e18b934134985674e3227416ba1d89c36f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 3.7 | 3 | 3 | [run](https://argusic.com/run/5102c720-01dc-47bc-9681-ed69fc491c21) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in PATH (go: not found)`
- 1 min: `dsnet init fails with 'permission denied' writing to /etc/dsnetconfig.json (no root/sudo available)`
- 1 min: `dsnet sync, report, and the sync-after-add step fail with 'operation not permitted' - requires root netlink access to WireGuard kernel interface`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
