# enroute

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/enroute-sh/enroute, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/enroute

## Pinned environment

- Project commit: `bc0dc6efce9cbbce9a5368e594a9b28f18a12d40`
- Test commit: `bc0dc6efce9cbbce9a5368e594a9b28f18a12d40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.4 to 9.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 9.4 | 2 | 2 | [run](https://argusic.com/run/be470dd8-4e7e-4331-8d3b-5421dc59c2ba) |

## What was observed on a clean machine

Attempt 1:

- `raft test file (5 tests) failed on first run: idle_repos_go_quiet, lagging_follower_catches_up_via_snapshot, members_are_every_logs_voters, replicated_push_and_failover all panicked with timeout/read-barrier errors`
- `crash test (acknowledged_writes_survive_sigkill) failed on first run: cluster did not become ready`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
