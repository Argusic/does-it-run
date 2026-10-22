# ESPAltherma

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/raomin/ESPAltherma, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/espaltherma

## Pinned environment

- Project commit: `c3b4286f829e1243aa88fe7dcb6dac4ea80a32ed`
- Test commit: `c3b4286f829e1243aa88fe7dcb6dac4ea80a32ed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.3 to 2.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 2.3 | 2 | 2 | [run](https://argusic.com/run/77d1a202-e692-46d9-8caf-f6257857a4e2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install platformio failed: externally-managed-environment (PEP 668) on Debian Python 3.12`
- 1 min: `Failed to create venv under /work (permission denied: directory is root-owned, user is runner)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
