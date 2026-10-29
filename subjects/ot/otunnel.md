# otunnel

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ooclab/otunnel, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/otunnel

## Pinned environment

- Project commit: `d1c82ee5d6b0a7f4076deb5422e3fedf192b2e66`
- Test commit: `d1c82ee5d6b0a7f4076deb5422e3fedf192b2e66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.6 to 2.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 2.6 | 1 | 1 | [run](https://argusic.com/run/fe871c2e-59b9-4f24-95ee-b07f12b0a5ef) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain not installed in container (go: not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
