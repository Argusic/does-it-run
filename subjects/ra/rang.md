# rang

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agauniyal/rang, licensed Unlicense, written in C++.

Evidence and recordings: https://argusic.com/subject/rang

## Pinned environment

- Project commit: `56419fe3348a475c8dd83852d907794cec0ec798`
- Test commit: `56419fe3348a475c8dd83852d907794cec0ec798`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.6 to 3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.6 | 1 | 1 | [run](https://argusic.com/run/fd1602a6-90ce-4bf9-b237-1cbaded722c3) |
| 2 | pass | 100 | 6 | 3 | 2 | 2 | [run](https://argusic.com/run/accb9552-1344-4f73-9629-39dbee6fa3e8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `doctest dependency not found by CMake , cmake could not find doctestConfig.cmake`

Attempt 2:

- 2 min: `doctest C++ test framework missing from system`
- 1 min: `test/CMakeLists.txt used '${doctest_FOUND} EQUAL 1' which fails with Finddoctest.cmake (string vs numeric comparison)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
