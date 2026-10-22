# flamingo-commerce

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/i-love-flamingo/flamingo-commerce, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/flamingo-commerce

## Pinned environment

- Project commit: `e09afeae8ea518cc6a5b73260bbcf398bd03a3a0`
- Test commit: `e09afeae8ea518cc6a5b73260bbcf398bd03a3a0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 20 | 7 | 1 | 0 | [run](https://argusic.com/run/e3097d35-4c2d-4821-b9c6-18bf910cf649) |

## What was observed on a clean machine

Attempt 1:

- `Docker-dependent Redis locker tests fail because Docker is unavailable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
