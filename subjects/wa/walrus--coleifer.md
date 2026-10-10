# walrus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coleifer/walrus, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/cd71dbab-3a62-49c6-9ff6-091d10d362f8

## Pinned environment

- Project commit: `81a4c03d71ca3ecc111d8cbac542a92d606128b5`
- Test commit: `81a4c03d71ca3ecc111d8cbac542a92d606128b5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6.5 | 6 | 2 | 2 | [run](https://argusic.com/run/cd71dbab-3a62-49c6-9ff6-091d10d362f8) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `redis-server not installed in container`
- 0.5 min: `pip externally-managed-environment on system Python`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
