# kopia

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kopia/kopia, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kopia

## Pinned environment

- Project commit: `661ba6e9c3296a711b6fdef857da64e1ff74a869`
- Test commit: `661ba6e9c3296a711b6fdef857da64e1ff74a869`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29.4 to 29.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 34 | 29.4 | 2 | 2 | [run](https://argusic.com/run/32c42219-1183-460c-abcc-a9880077ebcc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `go binary not installed in container`
- 1 min: `ssh-keygen missing causing SFTP test failures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
