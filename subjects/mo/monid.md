# monid

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/monid-ai/monid, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/monid

## Pinned environment

- Project commit: `b3e7b0c212e73039a691642e5624fc894096a1a7`
- Test commit: `b3e7b0c212e73039a691642e5624fc894096a1a7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 9.9 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15.1 | 0 | 0 | [run](https://argusic.com/run/aef3efd6-9e8d-4132-a2af-16791bb8a50c) |
| 2 | pass with mocks | 92 | 11 | 9.9 | 0 | 0 | [run](https://argusic.com/run/ffd6b9f1-d8f2-4da5-8768-324b08a05836) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
