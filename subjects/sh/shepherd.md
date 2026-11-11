# shepherd

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shepherd-agents/shepherd, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/shepherd

## Pinned environment

- Project commit: `d34d5ca334871dfcb5a3dc76dd78045829fa4e56`
- Test commit: `d34d5ca334871dfcb5a3dc76dd78045829fa4e56`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 22 to 33 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 33 | 3 | 3 | [run](https://argusic.com/run/b25e6102-51d1-4ddb-bf11-c830d2731691) |
| 2 | pass | 95 | 21 | 22 | 4 | 3 | [run](https://argusic.com/run/c9e1c849-e44a-4ccb-81a3-794e5b5274c6) |

## What was observed on a clean machine

Attempt 1:

- `Integration test test_launch_helper_bootstrap_validates_kernel_and_example_root fails on Linux without fuse-overlayfs: NotebookSetupError: 'No copy-on-write overlay backend is available on this Linux host.'`
- `Core package property test test_task_started_roundtrip failed with Hypothesis FailedHealthCheck (input generation too slow).`
- `shepherd/packages/dialect/tests/test_providers.py hangs indefinitely (timeout > 30s).`

Attempt 2:

- 1 min: `meta test expected shepherd.__version__ '0.3.0' but actual is '0.3.1'`
- 2 min: `integration test test_core_reexports expected __all__ without 'AmbientWorldAccessRefused' and 'AmbiguousTaskBody'`
- 2 min: `test_workspace_already_configured_raises_on_conflict expected an exception that no longer raises per design change`
- `vcs-core: 3 pre-existing mock failures (test_session_shell mock IPC, test_daemon_lifecycle FakeConnection missing getsockopt)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
