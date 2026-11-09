# adhd

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/UditAkhourii/adhd, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/adhd

## Pinned environment

- Project commit: `dd08acc38693127cd0ca2325fe6bf9579131ede1`
- Test commit: `dd08acc38693127cd0ca2325fe6bf9579131ede1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 4.8 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 13.6 | 0 | 0 | [run](https://argusic.com/run/ea284482-3abe-4a64-bce2-c6680680b6e5) |
| 2 | fail | 50 | 3 | 4.8 | 1 | 1 | [run](https://argusic.com/run/72d15942-9f2a-4e3a-87ba-e537cf451149) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
