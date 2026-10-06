# rsmq

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/smrchy/rsmq, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/rsmq

## Pinned environment

- Project commit: `7372ea1a060cabeb59a86a3846c597e043b5619a`
- Test commit: `7372ea1a060cabeb59a86a3846c597e043b5619a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.3 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 4.3 | 0 | 0 | [run](https://argusic.com/run/aa07f6b5-abb1-436d-a633-0a430f351de1) |
| 2 | pass | 100 | 6 | 6.2 | 2 | 2 | [run](https://argusic.com/run/2d98461b-28f0-4ea8-b102-58c6d39facf7) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js v18.19.1 installed but rsmq requires >=20`
- 3 min: `No redis-server available in container; fakeredis lacks EVAL support`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
