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
- Valid runs: 2; wall time 38.3 to 61.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10.6 | 38.3 | 6 | 6 | [run](https://argusic.com/run/7d8af1d4-9885-4957-935d-edf5f979651e) |
| 2 | pass with mocks | 92 | 60 | 61.3 | 5 | 5 | [run](https://argusic.com/run/ec23f412-4157-4160-9bdd-f2f08320100a) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `go not installed on system (needs >=1.25.3)`
- 1 min: `Python packages missing (robot, flask, psycopg2, etc)`
- 0.5 min: `mTLS certs missing for mock servers and PG server mode`
- 0.5 min: `mocked registry empty (test/registry-mocked/src)`
- 0.5 min: `sqlite3 CLI binary not available for export tests`
- `42 robot suite failures (512/554 pass)`

Attempt 2:

- 3 min: `Go 1.25.x not found in container`
- 2 min: `pip install failed: externally-managed-environment error`
- 2 min: `TLS certificates missing at test/server/mtls/credentials/`
- 1 min: `stackql_mcp_client binary not built by default build script`
- 1 min: `Registry mock Flask app hardcodes port 5000 in __main__`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
