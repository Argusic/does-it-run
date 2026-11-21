# vegas-pro-23-desktop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/angela-cook-1988/vegas-pro-23-desktop, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/vegas-pro-23-desktop

## Pinned environment

- Project commit: `52a0dde2fc4270aaaa163836be1e3abd26049a0e`
- Test commit: `52a0dde2fc4270aaaa163836be1e3abd26049a0e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2 to 2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2 | 1 | 1 | [run](https://argusic.com/run/5eb93135-1a81-4fe9-bec7-4905efdf289e) |

## What was observed on a clean machine

Attempt 1:

- `The C++ source file files/util.cpp contains a typo: '#include <cstdint>' should be '#include <cstdint>' -- this is not a valid header on Linux, but g++ still compiled it after resolving to a system header.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
