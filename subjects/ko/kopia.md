# kopia

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kopia/kopia, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kopia

## Pinned environment

- Project commit: `661ba6e9c3296a711b6fdef857da64e1ff74a869`
- Test commit: `661ba6e9c3296a711b6fdef857da64e1ff74a869`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 20.6 to 29.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 34 | 29.4 | 2 | 2 | [run](https://argusic.com/run/32c42219-1183-460c-abcc-a9880077ebcc) |
| 2 | pass | 93.33 | 12 | 20.6 | 9 | 6 | [run](https://argusic.com/run/2275ede7-455d-4231-be2f-785958957036) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `go binary not installed in container`
- 1 min: `ssh-keygen missing causing SFTP test failures`

Attempt 2:

- 2 min: `go compiler not found in PATH`
- 1 min: `npm audit failed on fast-uri v3.1.7`
- 2 min: `electron binary not installed (npm --ignore-scripts)`
- 2 min: `E2E test hardcoded /opt/KopiaUI which does not exist`
- 1 min: `chrome-sandbox not configured correctly (not root-owned in container)`
- 1 min: `dev-mode server path kopia_linux_amd64 does not exist`
- `SFTP tests fail because ssh-keygen and Docker are absent`
- `sparse-restore test fails on overlayfs (expected physical allocation mismatch)`
- `RPM packaging fails because rpmbuild is not installed and cannot be installed without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
