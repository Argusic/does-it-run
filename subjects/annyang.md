# annyang

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TalAter/annyang, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/annyang

## Pinned environment

- Project commit: `c31928ac9ae13df13fc7a370530065ea5a7502c1`
- Test commit: `c31928ac9ae13df13fc7a370530065ea5a7502c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.9 to 10.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 10.9 | 1 | 1 | [run](https://argusic.com/run/ef984f05-9627-405e-8159-814a281a16d7) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `vitest 4.x requires Node.js >=20 but container has Node v18.19.1; 145 tests failed with hook timeouts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
