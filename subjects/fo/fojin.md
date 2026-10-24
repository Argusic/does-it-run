# fojin

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xr843/fojin, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/fojin

## Pinned environment

- Project commit: `b38d9cc3c87e6f82a31a50e0337d131421266f02`
- Test commit: `b38d9cc3c87e6f82a31a50e0337d131421266f02`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 5 | 1 | 1 | [run](https://argusic.com/run/e5d5ebb9-4365-4758-a172-e985abff475e) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18 (system) can't build frontend , rolldown uses 'styleText' from 'node:util' which requires Node.js 21+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
