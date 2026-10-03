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
- Valid runs: 1; wall time 10.6 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 10.6 | 3 | 3 | [run](https://argusic.com/run/4b7bd71f-59c8-4eaa-869e-e83e53c5e507) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not found`
- 1 min: `libuuid-dev headers not found (only libuuid1 runtime library present)`
- 3 min: `default.theme not found at compile-time TASK_RCDIR path (/usr/local/share/doc/task/rc) during test execution`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
