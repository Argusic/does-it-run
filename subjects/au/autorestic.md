# autorestic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cupcakearmy/autorestic, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/autorestic

## Pinned environment

- Project commit: `496a8cc3afbbf25d8b019eae91d6bc0dce82591e`
- Test commit: `496a8cc3afbbf25d8b019eae91d6bc0dce82591e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.9 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 11.5 | 0 | 0 | [run](https://argusic.com/run/05f5552e-3577-46b8-8611-8c8d9ace3a3c) |
| 2 | pass | 100 | 8 | 2.9 | 3 | 3 | [run](https://argusic.com/run/bc5eaa2a-57f0-4dde-a348-6dcf7747c12f) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go binary not available in container`
- 1 min: `restic binary not available in container`
- 1 min: `autorestic install command requires write to /usr/local/bin (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
