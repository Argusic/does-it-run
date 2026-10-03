# perses

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/perses/perses, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/perses

## Pinned environment

- Project commit: `f8484aa20d71c0df9176bbde029908990b79c1f0`
- Test commit: `f8484aa20d71c0df9176bbde029908990b79c1f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 19.5 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/a061bd3f-f279-45fc-9d64-a663fb935086) |
| 2 | pass | 100 | 16 | 19.5 | 2 | 2 | [run](https://argusic.com/run/cb0d2af3-1c65-4b60-8896-47d44a0efbc5) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go 1.27.1 not installed`
- 2 min: `Node.js v18.19.1 was too old (needs >=24)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
