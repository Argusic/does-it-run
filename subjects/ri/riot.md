# riot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vcaesar/riot, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/riot

## Pinned environment

- Project commit: `0219e1c26ca1b7242add1e1a518552caf8d57f16`
- Test commit: `0219e1c26ca1b7242add1e1a518552caf8d57f16`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.2 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.2 | 0 | 0 | [run](https://argusic.com/run/cef61b75-2dca-4c9e-a800-22235af626f5) |
| 2 | pass | 100 | 18 | 12.4 | 3 | 3 | [run](https://argusic.com/run/a8682e24-f590-4071-b357-dafa2e401107) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `no Go toolchain in container (go: not found)`
- 2 min: `go.mod requires go 1.26.0 so initially fetched go1.24.4 (superset not satisfied)`
- 1 min: `I first ran 'riot snapshot <path> 1' on an index whose only snapshot is 2 and it printed a file-not-found error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
