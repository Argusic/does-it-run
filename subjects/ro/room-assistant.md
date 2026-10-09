# room-assistant

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mKeRix/room-assistant, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/room-assistant

## Pinned environment

- Project commit: `ed9a860e8ca2f481c76f11b66f632a30551d4416`
- Test commit: `ed9a860e8ca2f481c76f11b66f632a30551d4416`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 40.7 to 40.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 40.7 | 2 | 2 | [run](https://argusic.com/run/07418986-92b1-4c64-97b9-f9f83f35dbad) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Build failed: TS2307 - Cannot find module 'canvas'`
- 5 min: `Test suite failed: Could not locate native binding epoll.node for onoff`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
