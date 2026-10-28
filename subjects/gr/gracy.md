# gracy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/guilatrova/gracy, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gracy

## Pinned environment

- Project commit: `44df30beb31733c71ffae6759fae230588143d21`
- Test commit: `44df30beb31733c71ffae6759fae230588143d21`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 7 | 1 | 1 | [run](https://argusic.com/run/58a4b24d-0f3e-4745-abf9-ac09b85c951b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Python blocked by PEP 668 externally-managed environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
