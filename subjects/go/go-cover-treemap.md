# go-cover-treemap

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nikolaydubina/go-cover-treemap, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/go-cover-treemap

## Pinned environment

- Project commit: `5d57d47e825cc7c6e42c017816eafc4f0f3a88c2`
- Test commit: `5d57d47e825cc7c6e42c017816eafc4f0f3a88c2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.3 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 3.7 | 1 | 1 | [run](https://argusic.com/run/84a3da12-f8b5-44aa-912e-1b7e86da24d9) |
| 2 | pass | 100 | 2.5 | 2.3 | 2 | 2 | [run](https://argusic.com/run/4ee49304-1d64-4cd8-b409-20ae7391b122) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25.0 not found in PATH, 'go' command missing from container`

Attempt 2:

- 1.5 min: `Go binary not found in system , installed from official tarball`
- 0.5 min: `go test ./... fails on web/ package , imports syscall/js which is excluded on non-WASM targets`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
