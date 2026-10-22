# ProjectAtlas

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/styler-ai/ProjectAtlas, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/projectatlas

## Pinned environment

- Project commit: `8d28ac0a9fb6fb1b9d195928ab0ff8aa0cd004e6`
- Test commit: `8d28ac0a9fb6fb1b9d195928ab0ff8aa0cd004e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.6 to 35.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 1.5 | 35.6 | 4 | 3 | [run](https://argusic.com/run/cae2ba7a-3a52-4909-8bd8-a8d5445f544a) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Flaky test payload_observation_detects_same_size_same_mtime_change_epoch in parser_supervisor.rs , ctime has ~1ms granularity on overlayfs, write+set_times can complete within same ctime tick`
- 5 min: `Flaky test linux_currentness_probe_detects_native_policy_drift in parser_supervisor.rs , same ctime granularity issue`
- 8 min: `Git 2.43 does not support --ref-format=reftable; test structural_discovery_covers_real_git_worktree_lifecycle_matrix fails`
- 5 min: `2 e2e_delivery tests (pre_push_candidate_rejects_ignored_linked_document_outside_tree, pre_push_dispatch_follows_pushed_remote_targets) require GitHub remote push and IssueOps dispatch infrastructure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
