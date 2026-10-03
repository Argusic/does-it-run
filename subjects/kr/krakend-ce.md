# krakend-ce

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/krakend/krakend-ce, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/krakend-ce

## Pinned environment

- Project commit: `dc4321e9b4278fc28519565906d413e2b392ca0d`
- Test commit: `dc4321e9b4278fc28519565906d413e2b392ca0d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 4.1 | 2 | 2 | [run](https://argusic.com/run/3670ed6e-4bcd-449f-818c-907c869c6e5c) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `go binary not found in container`
- 0.5 min: `wget not available for Makefile schema fetch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
