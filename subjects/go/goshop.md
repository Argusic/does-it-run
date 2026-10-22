# goshop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/quangdangfit/goshop, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/goshop

## Pinned environment

- Project commit: `3990165dd9b40731ae3e793e84895f0b8ae31839`
- Test commit: `3990165dd9b40731ae3e793e84895f0b8ae31839`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 7.5 | 3 | 3 | [run](https://argusic.com/run/98037571-079d-4ebd-aed3-5da28eda63c9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in environment`
- 0.5 min: `Missing config.yaml (config_test.go expects one)`
- 2 min: `Web frontend vitest/vite build fails with Node.js 18 (need Node 22+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
