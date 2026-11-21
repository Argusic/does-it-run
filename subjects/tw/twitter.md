# twitter

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/atymic/twitter, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/twitter

## Pinned environment

- Project commit: `bc0dd97f8c67fa55ec86ef9cbfd02d21717244d2`
- Test commit: `bc0dd97f8c67fa55ec86ef9cbfd02d21717244d2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 0.3 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 3.4 | 0 | 0 | [run](https://argusic.com/run/d2356b57-a485-4827-9d81-905f72b4f931) |
| 2 | fail | 20 | n/a | 0.3 | 0 | 0 | [run](https://argusic.com/run/f25e6a1b-e1b7-407c-b4da-bb4879753e7a) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
