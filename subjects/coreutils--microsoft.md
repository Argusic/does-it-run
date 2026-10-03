# coreutils

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/coreutils, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/4efbff6a-8a1a-4942-9f27-dfbde5e786e4

## Pinned environment

- Project commit: `09f098d288f08a8071acf6dce9671a63ffb2e575`
- Test commit: `09f098d288f08a8071acf6dce9671a63ffb2e575`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.4 to 27.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 27.4 | 10 | 10 | [run](https://argusic.com/run/4efbff6a-8a1a-4942-9f27-dfbde5e786e4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Rust toolchain installed`
- 0.5 min: `Git submodules not initialized`
- 2 min: `ntsort/sort.c requires windows.h (Windows-only native sort)`
- 1 min: `winresource requires Windows SDK for manifest compilation`
- 2 min: `ntfind crate uses windows_sys for DOS-style find command`
- 3 min: `main.rs unconditionally used windows_sys types (Console, TerminateProcess, etc.)`
- 1 min: `manager.rs is Windows-only (registry, pipes, shell integration)`
- 1 min: `stat.rs missing metadata_get_time import on Linux (was only imported on Windows)`
- 1 min: `stat.rs used entries::gid2grp/uid2usr without importing uucore::entries`
- 1 min: `binary_path/name functions from upstream coreutils crate not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
