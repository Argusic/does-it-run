# gost

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/go-gost/gost, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gost

## Pinned environment

- Project commit: `e9fab9587288b82ce8a1a9b8f07326f41b155935`
- Test commit: `e9fab9587288b82ce8a1a9b8f07326f41b155935`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 7.7 | 1 | 1 | [run](https://argusic.com/run/54c33aa0-a401-4495-8d66-cfd175fa646e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed (go: not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
