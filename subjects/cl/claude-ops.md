# claude-ops

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Lifecycle-Innovations-Limited/claude-ops, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/claude-ops

## Pinned environment

- Project commit: `a1ff10f46dddf1bfc5c4881d5c94c939d05a21e4`
- Test commit: `a1ff10f46dddf1bfc5c4881d5c94c939d05a21e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 50.3 to 50.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.02 | 50.3 | 4 | 4 | [run](https://argusic.com/run/eba20b95-89ec-4702-985d-4cdc8909b55b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test-pid-performance-monitor.py: on a 192-CPU machine, load threshold (NCPU*2=384) never reached by test loads (100), causing false failures in qos/pressure tests`
- 2 min: `test-staged-enrollment.mjs: uses import.meta.dirname (Node 20+ API) not available in Node 18`
- 2 min: `test-coordination-provisioning.mjs: installer script (install-account-rotator-linux.sh) checks for Node 20+ and fails on Node 18`
- 10 min: `test-post-update-migrate-current-guard.sh: rsync not installed on this container; 2 of 6 test cases (rsync-path, allow-forward-update) test rsync-specific --delete/exclude behavior`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
