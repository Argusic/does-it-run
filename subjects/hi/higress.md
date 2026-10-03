# higress

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/higress-group/higress, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/higress

## Pinned environment

- Project commit: `22368f1e7a284ded69607334ba08fbb5d2a7ee5e`
- Test commit: `22368f1e7a284ded69607334ba08fbb5d2a7ee5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 14.9 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/d928bb9d-7731-4d26-8cb8-11f36b01565d) |
| 2 | fail | 80 | 13 | 14.9 | 3 | 3 | [run](https://argusic.com/run/e90ed70e-bb4e-470e-8f4d-42a2cc3849ec) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Go 1.26 not installed in container`
- 1 min: `Git submodules not initialized`
- 3 min: `external/ directories not set up (prebuild)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
