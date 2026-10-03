# OpenResearch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alphaXiv/OpenResearch, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/openresearch

## Pinned environment

- Project commit: `f336b121525d99364e2dee4fe90b2784894a54e6`
- Test commit: `f336b121525d99364e2dee4fe90b2784894a54e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.3 to 14.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 14.3 | 1 | 1 | [run](https://argusic.com/run/176026a2-fe9b-475b-803f-3227e9ea5d8f) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `ssh-keygen not found in container (missing openssh-client package)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
