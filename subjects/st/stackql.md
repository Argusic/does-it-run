# stackql

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/stackql/stackql, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/stackql

## Pinned environment

- Project commit: `adc09567d4ba98870e46dae94332c55e03a5a212`
- Test commit: `adc09567d4ba98870e46dae94332c55e03a5a212`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 38.3 to 38.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10.6 | 38.3 | 6 | 6 | [run](https://argusic.com/run/7d8af1d4-9885-4957-935d-edf5f979651e) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `go not installed on system (needs >=1.25.3)`
- 1 min: `Python packages missing (robot, flask, psycopg2, etc)`
- 0.5 min: `mTLS certs missing for mock servers and PG server mode`
- 0.5 min: `mocked registry empty (test/registry-mocked/src)`
- 0.5 min: `sqlite3 CLI binary not available for export tests`
- `42 robot suite failures (512/554 pass)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
