# parlor

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fikrikarim/parlor, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/parlor

## Pinned environment

- Project commit: `da1ddf1f3e1a7ea04f69df24e98541ab5c402ccf`
- Test commit: `da1ddf1f3e1a7ea04f69df24e98541ab5c402ccf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 76.8 to 76.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 22 | 76.8 | 5 | 5 | [run](https://argusic.com/run/6cfbcde9-eb24-4ccc-b8cd-0e6fc8479fac) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No uv pre-installed in container`
- 2 min: `Server failed to bind on localhost (IPv6 resolved to ::1, not supported)`
- 1 min: `Stale ports in TIME_WAIT across test runs`
- `CPU inference too slow for e2e test suite (70s per turn)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
