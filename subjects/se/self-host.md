# self-host

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ajnart/self-host, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/self-host

## Pinned environment

- Project commit: `865e7a0bddc92440becf433884030568d0621e5f`
- Test commit: `865e7a0bddc92440becf433884030568d0621e5f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 2.6 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 8.3 | 1 | 1 | [run](https://argusic.com/run/6c534891-8372-486d-8767-44bbdf848dd6) |
| 2 | fail | 80 | 0.5 | 2.6 | 0 | 0 | [run](https://argusic.com/run/99512fc5-a4a7-4942-bf46-ad4646fb71d2) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `Go compiler not found in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
