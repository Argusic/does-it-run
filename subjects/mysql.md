# mysql

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/go-sql-driver/mysql, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/mysql

## Pinned environment

- Project commit: `789a82a35d04f8ab5a7b28707615ef8bf9d4f09b`
- Test commit: `789a82a35d04f8ab5a7b28707615ef8bf9d4f09b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.8 to 11.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9.48 | 11.8 | 2 | 2 | [run](https://argusic.com/run/54b2b8e2-0aa1-4c69-8520-e6a27fb2236f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in environment`
- 5 min: `No MySQL server available in container for integration tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
