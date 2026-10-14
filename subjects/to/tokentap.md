# tokentap

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jmuncor/tokentap, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tokentap

## Pinned environment

- Project commit: `ac4b8b95a2d930a2215a08df191d4553b6ab44e5`
- Test commit: `ac4b8b95a2d930a2215a08df191d4553b6ab44e5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.4 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.4 | 1 | 1 | [run](https://argusic.com/run/c7425f58-1be7-4295-8262-09946a4d5285) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install -e . failed with 'error: externally-managed-environment' (PEP 668) on the system Python`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
