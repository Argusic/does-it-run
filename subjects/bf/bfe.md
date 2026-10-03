# bfe

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bfenetworks/bfe, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/bfe

## Pinned environment

- Project commit: `c95df40a3af93d3a3b8e719e47357740bb5e8865`
- Test commit: `c95df40a3af93d3a3b8e719e47357740bb5e8865`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 6.2 | 1 | 1 | [run](https://argusic.com/run/95c38d98-4ed5-460e-bff6-6f637fbdfd74) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go 1.22.9 not pre-installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
