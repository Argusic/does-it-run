# ursina

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pokepetter/ursina, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ursina

## Pinned environment

- Project commit: `807384a495a9debb3c66b601dafea552a78fc77b`
- Test commit: `807384a495a9debb3c66b601dafea552a78fc77b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.9 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 9.9 | 2 | 2 | [run](https://argusic.com/run/02263ecb-fafe-48c1-8f3b-bf24f88d6df3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `externally-managed-environment (PEP 668) prevents system-wide pip install`
- `Ursina object has no attribute 'quit'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
