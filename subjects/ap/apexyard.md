# apexyard

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/me2resh/apexyard, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/apexyard

## Pinned environment

- Project commit: `fa6911078bb3c91af457290cd2c7e8bd91843746`
- Test commit: `fa6911078bb3c91af457290cd2c7e8bd91843746`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 64.4 to 64.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 64.4 | 9 | 9 | [run](https://argusic.com/run/780138c7-49e0-4a98-b686-21d58a9f53b6) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Tests hang waiting for gh CLI (GitHub CLI); 3 tests timed out at 120s`
- 1 min: `yq (pip version) can't parse -o=json flag; 2 test failures`
- 1 min: `pyyaml missing; 6 tracker tests skipped critical cases`
- 1 min: `rsync not installed; scaffold test fails at line 184`
- `test_require_migration_ticket.sh: 1 of 85 cases (#1182 selection parity) needs parent git commit`
- `test_process_bpmn.sh: Node 18.19.1 vs required >=20.12 for bpmnlint`
- `test_block_protected_target_writes.sh: matrix-spawned subprocesses exceed 120s timeout`
- `test_scaffold_generate.sh: hangs after rsync-fix on network/process isolation step`
- `test_records_lint_slice_merge_base_drift.sh: no ancestor commit for base comparison`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
