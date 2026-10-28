# brotab

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/balta2ar/brotab, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/brotab

## Pinned environment

- Project commit: `6c71e1013972b0d73f29e92239a695526e2e9c58`
- Test commit: `6c71e1013972b0d73f29e92239a695526e2e9c58`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.7 to 2.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.7 | 3 | 3 | [run](https://argusic.com/run/c2e8a673-90ce-4ee0-add6-b1a93b8514ef) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `externally-managed-environment blocks system-wide pip install`
- 1 min: `psutil==5.8.0 requires Python.h to build from source (no python3-dev installed)`
- 1 min: `pinned deps in requirements/base.txt (Flask==2.2.2, requests==2.24.0, Werkzeug<3.0, setuptools==75.8.0) conflict with available wheels`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
