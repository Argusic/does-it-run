# openclip

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/linzzzzzz/openclip, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/openclip

## Pinned environment

- Project commit: `028962794838db31d938f7d5d4c6513c06a0cf1b`
- Test commit: `028962794838db31d938f7d5d4c6513c06a0cf1b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.6 | 0 | 0 | [run](https://argusic.com/run/bc4bdc62-2c4e-4e73-bc64-8f90a58fe5a9) |
| 2 | pass with mocks | 92 | 8 | 4 | 0 | 0 | [run](https://argusic.com/run/55c8fea3-7dcc-4306-b5cd-15244ab148d0) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
