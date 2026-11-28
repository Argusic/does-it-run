# telescope

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iamtelescope/telescope, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/telescope

## Pinned environment

- Project commit: `ea0359c5bc089f0797a7a18cc23dc4714a8f37a9`
- Test commit: `ea0359c5bc089f0797a7a18cc23dc4714a8f37a9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.3 to 3.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 3.3 | 1 | 1 | [run](https://argusic.com/run/6100ff60-9e35-413a-a271-fd2841d70ec5) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `test config.yaml missing ALLOWED_HOSTS and DEBUG causing runserver to fail with CommandError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
