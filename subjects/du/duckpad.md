# duckpad

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hugues31/duckpad, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/duckpad

## Pinned environment

- Project commit: `5df0286f869a9352c111a7fa822d363da305e0b4`
- Test commit: `5df0286f869a9352c111a7fa822d363da305e0b4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 28.7 to 37.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 28.7 | 0 | 0 | [run](https://argusic.com/run/a31781ad-bcfd-4f47-a056-d1d593d2d334) |
| 2 | pass | 100 | 2 | 37.9 | 2 | 2 | [run](https://argusic.com/run/7cf91a9c-ca32-40a4-9301-bf18ad2298cf) |

## What was observed on a clean machine

Attempt 2:

- `git-cliff binary not found (test_release.py fails)`
- `OpenSSH client/server not available (test_git_ssh.py skipped)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
