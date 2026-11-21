# updo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Owloops/updo, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/updo

## Pinned environment

- Project commit: `97998eae455a6f54d3da2119723d2857ab4aab0f`
- Test commit: `97998eae455a6f54d3da2119723d2857ab4aab0f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.4 to 2.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.4 | 2 | 2 | [run](https://argusic.com/run/d8718137-0090-4594-844d-4a744685020f) |
| 2 | pass | 100 | 2 | 2.6 | 2 | 2 | [run](https://argusic.com/run/8ab25bc0-a3cc-474d-8ef1-22251d347940) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go 1.27+ not installed in container`
- 0.3 min: `"zip" command not available (required by Makefile for Lambda ZIP)`

Attempt 2:

- 1 min: `Go 1.27.4 was not installed in the container`
- 1 min: `zip command not found for Lambda ZIP creation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
