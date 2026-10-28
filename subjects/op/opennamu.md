# openNAMU

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openNAMU/openNAMU, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/opennamu

## Pinned environment

- Project commit: `deb09d4a951729a5fa72cf9d10ec395586bc47b0`
- Test commit: `deb09d4a951729a5fa72cf9d10ec395586bc47b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.2 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 16.2 | 3 | 3 | [run](https://argusic.com/run/be090860-2077-4c92-b9b6-2feb230bee8f) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `go: not found in container`
- 3 min: `go test ./... scanned the Go toolchain source tree that was inside the repo module`
- 5 min: `POST /edit/Test returned error page 'CAPTCHA를 통과하세요'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
