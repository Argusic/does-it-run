# ghs

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/seart-group/ghs, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/ghs

## Pinned environment

- Project commit: `9f108a5799e77b990e0e1abfa9563a92ec28cc2b`
- Test commit: `9f108a5799e77b990e0e1abfa9563a92ec28cc2b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.6 to 15.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 15.6 | 2 | 2 | [run](https://argusic.com/run/e987b69e-149b-4dd0-923e-151c61bf2c3c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Java and Maven not in container`
- 7 min: `MySQL database required but not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
