# smart-home

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/denysdovhan/smart-home, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/smart-home

## Pinned environment

- Project commit: `12665d8a09e30f1f1d93163f8aad94437fc0328f`
- Test commit: `12665d8a09e30f1f1d93163f8aad94437fc0328f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 5.4 | 2 | 2 | [run](https://argusic.com/run/6597f228-1ff7-4614-ae9c-6d9f25e1c98b) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `uv not found in PATH`
- `Docker not available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
