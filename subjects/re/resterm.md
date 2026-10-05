# resterm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/unkn0wn-root/resterm, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/resterm

## Pinned environment

- Project commit: `1bf4880dc68198cc8384121c4735d90d6453b77a`
- Test commit: `1bf4880dc68198cc8384121c4735d90d6453b77a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.2 to 21.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 21.2 | 2 | 2 | [run](https://argusic.com/run/472a6cca-a9f4-4c22-a9db-52d3be89e9c3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go (golang) compiler not installed`
- 5 min: `internal/mock tests failed on overlay FS due to identical mtime_ns for rapid same-size writes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
