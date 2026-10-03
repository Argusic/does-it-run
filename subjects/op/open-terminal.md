# open-terminal

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-webui/open-terminal, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/open-terminal

## Pinned environment

- Project commit: `b58442aa8599755525878f917b621e0145b0e8f7`
- Test commit: `b58442aa8599755525878f917b621e0145b0e8f7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 8 | 1 | 1 | [run](https://argusic.com/run/62dc475b-bedb-4cfd-8f30-09917240fbdf) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install -e . failed: externally-managed-environment (Debian PEP 668)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
