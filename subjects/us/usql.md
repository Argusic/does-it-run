# usql

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xo/usql, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/usql

## Pinned environment

- Project commit: `687d7b5deaa19ed36adffc9158e8e85fa7828a1b`
- Test commit: `687d7b5deaa19ed36adffc9158e8e85fa7828a1b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.2 to 13.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 10 | 13.2 | 4 | 2 | [run](https://argusic.com/run/613bb600-effa-470f-b1bc-ec71e4e1204f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in container`
- 1 min: `Test recording expects PAGER='less' but container has PAGER='more'`
- `Docker-dependent tests (informationschema, postgres, sqlserver) fail - no Docker socket available`
- `ODBC driver build fails - missing unixODBC development headers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
