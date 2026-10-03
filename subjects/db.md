# db

**Verdict: runs with mocks.** Argusic Score 84.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/upper/db, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/db

## Pinned environment

- Project commit: `dd97b4b4d5c6dcdd837c2011c08c3e1745e75da0`
- Test commit: `dd97b4b4d5c6dcdd837c2011c08c3e1745e75da0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 6 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 75 | 1.5 | 9.8 | 4 | 3 | [run](https://argusic.com/run/d6d690c2-6235-4c90-a317-a6078378f239) |
| 2 | pass with mocks | 85.33 | 4 | 14 | 3 | 2 | [run](https://argusic.com/run/310e1aeb-20d7-4848-adf4-70bfc5ea915b) |
| 3 | pass with mocks | 92 | 2.5 | 6 | 3 | 3 | [run](https://argusic.com/run/513bede8-2461-4b71-b69c-344644870aea) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go 1.23 not installed`
- 0.1 min: `Missing internal/testsuite package referenced by ql and sqlite adapter tests`
- 0.1 min: `Sqlite adapter tests fail without DB_NAME env var`
- `tests/ package requires Docker and Ansible which are unavailable`

Attempt 2:

- 2 min: `Go 1.23.2 not installed in container`
- 1 min: `internal/testsuite package missing (needed by adapter/sqlite, adapter/ql tests)`
- `integration tests in tests/ require Docker + Ansible (ansible-playbook not found, no Docker)`

Attempt 3:

- 2 min: `Go 1.23 not installed in container`
- 0.5 min: `Missing internal/testsuite package referenced by adapter/ql and adapter/sqlite tests`
- `tests/ directory integration tests fail: ansible-playbook not found (Docker not available)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
