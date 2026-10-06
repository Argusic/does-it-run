# quivr

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/The-Vibe-Company/quivr, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/quivr

## Pinned environment

- Project commit: `f247cb21bbec52bf1c751191ddc99cc350ffa667`
- Test commit: `f247cb21bbec52bf1c751191ddc99cc350ffa667`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 16.6 | 4 | 4 | [run](https://argusic.com/run/7d55a71b-71db-4384-816e-66e9b783f0c2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed`
- 3 min: `Missing Python dependencies for tests`
- 5 min: `Docker not available`
- `modal module not importable in eval tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
