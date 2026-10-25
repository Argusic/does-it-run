# scout

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coleifer/scout, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/8a62891e-5dc4-4856-8b67-fddd535d7032

## Pinned environment

- Project commit: `42694869866584c79435783c08273c8704761d15`
- Test commit: `42694869866584c79435783c08273c8704761d15`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2 to 2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.2 | 2 | 2 | 2 | [run](https://argusic.com/run/8a62891e-5dc4-4856-8b67-fddd535d7032) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `python3 not linked as 'python' on Ubuntu 24.04`
- 1 min: `PEP 668 externally-managed-environment prevents system-wide pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
