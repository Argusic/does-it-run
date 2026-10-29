# android-ad-cleaner

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rddmwmddr/android-ad-cleaner, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/android-ad-cleaner

## Pinned environment

- Project commit: `90c267618b10d949f3052a510e90f4dc4ee0a803`
- Test commit: `90c267618b10d949f3052a510e90f4dc4ee0a803`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 5.1 | 4 | 4 | [run](https://argusic.com/run/37ce83ac-dc32-4e62-87e9-c883d78d7229) |

## What was observed on a clean machine

Attempt 1:

- 0.25 min: `No adb binary found; tool/run.py exits at import when adb is missing`
- 1.5 min: `pip refused system install: externally-managed-environment (PEP 668)`
- 1.5 min: `pywebview had no GUI toolkit (no gi, no qtpy, no Qt)`
- 2 min: `Qt xcb platform plugin failed: system libxcb-cursor0 missing; no root for apt`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
