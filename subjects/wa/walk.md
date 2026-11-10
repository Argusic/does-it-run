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
- Valid runs: 2; wall time 14.6 to 21.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 21.7 | 1 | 1 | [run](https://argusic.com/run/3f729128-b0ed-48ac-a026-0683e083eeba) |
| 2 | pass | 100 | 19.7 | 14.6 | 3 | 3 | [run](https://argusic.com/run/fdacda90-efdb-4b3a-be15-fbe104d0327b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go toolchain not installed in container`

Attempt 2:

- 10 min: `V compiler (vlang) installed unnecessarily - this is a Go project, not a V project`
- 5 min: `The V compiler from master branch had broken cached .vh headers preventing self-compilation`
- 2 min: `No TTY available to run the interactive terminal app`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
