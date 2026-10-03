# freellmapi

**Verdict: runs.** Argusic Score 70.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tashfeenahmed/freellmapi, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/freellmapi

## Pinned environment

- Project commit: `47c3a451e88242a97d274777a29a4dbf289e3e17`
- Test commit: `47c3a451e88242a97d274777a29a4dbf289e3e17`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run, no run possible
- Valid runs: 3; wall time 6.4 to 31.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 9.9 | 1 | 1 | [run](https://argusic.com/run/6b6ab6f4-9bfc-4b30-b1ca-eb425751bd0d) |
| 2 | pass | 100 | 33 | 31.2 | 2 | 2 | [run](https://argusic.com/run/c7d53941-eae2-4d82-ab22-65a2504bc639) |
| 3 | fail | 20 | n/a | 6.4 | 0 | 0 | [run](https://argusic.com/run/30fced1e-035c-4917-90c1-cc0b989424fa) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js was v18.19.1 but project requires >=20.18.0`

Attempt 2:

- 1 min: `Node.js v18.19.1 in container, project requires >=20.18.0`
- 1 min: `Missing @rolldown/binding-linux-x64-gnu native module blocked client build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
