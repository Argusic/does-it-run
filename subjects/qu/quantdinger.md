# QuantDinger

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenByteInc/QuantDinger, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/quantdinger

## Pinned environment

- Project commit: `a9c722e024760c490e9f348fd0cca333b170b8c8`
- Test commit: `a9c722e024760c490e9f348fd0cca333b170b8c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 6.7 | 0 | 0 | [run](https://argusic.com/run/cb8a1928-6f90-427d-a8ea-7d6f5996dedd) |
| 2 | pass with mocks | 92 | 2 | 4.7 | 0 | 0 | [run](https://argusic.com/run/a919bef4-ebb3-42fd-a172-55f651e2d4c0) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
