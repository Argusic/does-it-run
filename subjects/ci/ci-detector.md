# ci-detector

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OndraM/ci-detector, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/ci-detector

## Pinned environment

- Project commit: `3ecbdd55b277640011738da030756783e7db46a1`
- Test commit: `3ecbdd55b277640011738da030756783e7db46a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.07 | 4 | 1 | 1 | [run](https://argusic.com/run/145b9e74-b3d2-4938-a7db-d2c1f980686e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP and Composer not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
