# sloth

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/slok/sloth, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/sloth

## Pinned environment

- Project commit: `8a3be4fab79defa4448d09d91b48422615980b05`
- Test commit: `8a3be4fab79defa4448d09d91b48422615980b05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 9.1 | 1 | 1 | [run](https://argusic.com/run/abbb945b-5b7e-4b24-af41-cb2c004f2cfc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
