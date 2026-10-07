# actionbook

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/actionbook/actionbook, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/actionbook

## Pinned environment

- Project commit: `0e31254cc10a1fe0b57faa318ac0823500f42a40`
- Test commit: `0e31254cc10a1fe0b57faa318ac0823500f42a40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.4 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 13.4 | 4 | 4 | [run](https://argusic.com/run/57d3d662-a209-4f9d-8eed-9a8c1ec6adcb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm was not pre-installed in the container`
- 3 min: `Rust toolchain not installed (needed for packages/cli)`
- 2 min: `tools-ai-sdk tests failed , mock exported 'getActionByIdDescription'/'getActionByIdSchema' but code imports 'getActionByAreaIdDescription'/'getActionByAreaIdSchema'`
- `CLI Rust lib test 'diagnose_port_holder_returns_pid_for_occupied' fails , depends on 'lsof' (not installed in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
