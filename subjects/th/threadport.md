# threadport

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Frankie-Xu/threadport, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/threadport

## Pinned environment

- Project commit: `249363bfbb8764d84e863dcd330e5389178a33a4`
- Test commit: `249363bfbb8764d84e863dcd330e5389178a33a4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.4 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.2 | 4.4 | 2 | 2 | [run](https://argusic.com/run/2a21cf9b-c4a8-4f1d-b6b6-ad223aaeea12) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18 is installed but the project requires Node >=24`
- 1.5 min: `Test control-plane.test.ts uses hardcoded expiry date '2026-09-30' which is past current date (2026-10-31), causing receipt status to be 'expired' instead of 'pending'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
