# ospec

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/clawplays/ospec, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ospec

## Pinned environment

- Project commit: `be449f2ce6986c62410a34b3bd4521d2f952a19c`
- Test commit: `be449f2ce6986c62410a34b3bd4521d2f952a19c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 4.8 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1.2 | 4.8 | 0 | 0 | [run](https://argusic.com/run/52fe2762-09d3-4024-b1f5-13269d1ea0e2) |
| 2 | pass with mocks | 92 | 4 | 5 | 2 | 2 | [run](https://argusic.com/run/7e00c7a4-afcb-4124-ba05-4a40fb5bf9c7) |

## What was observed on a clean machine

Attempt 2:

- `vitest 4.x requires Node 20+ but environment has Node 18.19.1; rolldown uses 'styleText' from 'node:util' not available in Node 18`
- `npm link fails with EACCES: permission denied to /usr/local/lib/node_modules/@clawplays`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
