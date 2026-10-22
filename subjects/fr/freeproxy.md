# freeproxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CharlesPikachu/freeproxy, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/freeproxy

## Pinned environment

- Project commit: `a32e93087029f363f007e93d6ee738cdc1f6d85f`
- Test commit: `a32e93087029f363f007e93d6ee738cdc1f6d85f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.1 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 3.1 | 3 | 3 | [run](https://argusic.com/run/569c57b2-6660-4880-935f-dcccae84e2e1) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `'python' binary not found; only python3 available`
- 2 min: `externally-managed-environment pip error on Debian`
- 0.5 min: `Missing SOCKS support for proxy protocol`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
