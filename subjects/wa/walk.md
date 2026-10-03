# walk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/antonmedv/walk, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/walk

## Pinned environment

- Project commit: `bf802ef9ee4b7895f88316138372b8356ad7afdb`
- Test commit: `bf802ef9ee4b7895f88316138372b8356ad7afdb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.7 to 21.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 21.7 | 1 | 1 | [run](https://argusic.com/run/3f729128-b0ed-48ac-a026-0683e083eeba) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go toolchain not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
