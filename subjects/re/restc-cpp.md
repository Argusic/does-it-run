# restc-cpp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jgaa/restc-cpp, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/restc-cpp

## Pinned environment

- Project commit: `a8cd803d097f194ba7ad044761bfeb93943d0664`
- Test commit: `a8cd803d097f194ba7ad044761bfeb93943d0664`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.8 to 15.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 15.8 | 3 | 3 | [run](https://argusic.com/run/12b89c91-34df-48ed-888d-fd75ca47f3de) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Boost libraries not installed on system (no root)`
- 3 min: `zlib1g-dev not installed (no root)`
- 4 min: `Functional tests require Docker containers (nginx, json-server, squid, socks) not available in this environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
