# taskwarrior

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GothenburgBitFactory/taskwarrior, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/taskwarrior

## Pinned environment

- Project commit: `9956cdfc674ec33d758675b7fab532c48ed8d555`
- Test commit: `9956cdfc674ec33d758675b7fab532c48ed8d555`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10.6 to 17.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 10.6 | 3 | 3 | [run](https://argusic.com/run/4b7bd71f-59c8-4eaa-869e-e83e53c5e507) |
| 2 | pass | 100 | 18 | 17.1 | 4 | 4 | [run](https://argusic.com/run/a3bd4271-0566-4550-b8ef-2ae7fb3cc9ea) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not found`
- 1 min: `libuuid-dev headers not found (only libuuid1 runtime library present)`
- 3 min: `default.theme not found at compile-time TASK_RCDIR path (/usr/local/share/doc/task/rc) during test execution`

Attempt 2:

- 1 min: `Rust toolchain not installed`
- 3 min: `libuuid development headers missing, cannot install uuid-dev (no root)`
- 1 min: `Local uuid header incomplete, missing uuid_t typedef`
- 1 min: `Cached CMake build referenced old Rust toolchain 1.88.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
