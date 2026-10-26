# xiryn

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SouravBeraAkaSpeed/xiryn, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/xiryn

## Pinned environment

- Project commit: `0a55cd9ecdc9f2d8dbb7ff057226607613dcc64b`
- Test commit: `0a55cd9ecdc9f2d8dbb7ff057226607613dcc64b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 5.8 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 7 | 5.8 | 1 | 1 | [run](https://argusic.com/run/c57e5c23-b477-4d6b-b03c-43400c5a690c) |
| 2 | pass with mocks | 92 | 4 | 6 | 2 | 2 | [run](https://argusic.com/run/58d614ba-7afb-4180-8b8c-6ae395508cce) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.19.1 installed but project requires >=20.9.0 (.nvmrc: 22)`

Attempt 2:

- 1 min: `Node.js v18.19.1 was too old (needs >=20.9)`
- 2 min: `Next.js 16.4.0 had a known security vulnerability that blocked the build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
