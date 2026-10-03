# dockly

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lirantal/dockly, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dockly

## Pinned environment

- Project commit: `572698cbcb5c712dfc7b1a8c33956380a7c8dd99`
- Test commit: `572698cbcb5c712dfc7b1a8c33956380a7c8dd99`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13.2 | 7.2 | 2 | 2 | [run](https://argusic.com/run/e94527f1-d2fe-4193-a67e-5dee54821e78) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js version mismatch: package.json requires >=24.0.0 but container has v18.19.1`
- 5 min: `No Docker daemon socket available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
