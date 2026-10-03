# Zappa

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zappa/Zappa, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/zappa

## Pinned environment

- Project commit: `e9ecb1feea14974f7bd76a908ca22ba1c9860d36`
- Test commit: `e9ecb1feea14974f7bd76a908ca22ba1c9860d36`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 37.1 to 39.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 39.7 | 0 | 0 | [run](https://argusic.com/run/821b259a-2e45-4e4d-b8da-09d6c958ded8) |
| 2 | pass with mocks | 92 | 1.5 | 37.1 | 2 | 2 | [run](https://argusic.com/run/da8c1547-d0fa-4b41-a538-0f5afaf3ecb9) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `VIRTUAL_ENV not set causes Path(None) TypeError in test_copy_editable_packages before skip check runs`
- 5 min: `Zappa.__init__ with load_credentials=True creates 16 boto3 clients, each taking ~2s for endpoint resolution, causing 30s+ hangs without real AWS or per-service placebo data`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
