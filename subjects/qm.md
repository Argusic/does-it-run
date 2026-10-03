# qm

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yc-software/qm, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/qm

## Pinned environment

- Project commit: `8adee4b06a595b061977de094208e5d8625b50b2`
- Test commit: `8adee4b06a595b061977de094208e5d8625b50b2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 12.6 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 12.6 | 0 | 0 | [run](https://argusic.com/run/bcc89bf7-631c-4e98-859e-88ef771925ae) |
| 2 | pass with mocks | 92 | 2 | 27.3 | 3 | 3 | [run](https://argusic.com/run/7be5465c-9d57-4fd6-a8ff-154be8d72a1e) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js 18.19.1 installed, project requires >=24.15.0`
- 1 min: `Connector SDK bundle missing for some tests`
- `2 dev-supervisor-child tests fail on IPv6/port ownership assertion (timing-sensitive dev tool tests)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
