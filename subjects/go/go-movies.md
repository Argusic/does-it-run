# go-movies

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hezhizheng/go-movies, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/go-movies

## Pinned environment

- Project commit: `d1cce37d5990644edf4c5f7fe2dfd254140167f3`
- Test commit: `d1cce37d5990644edf4c5f7fe2dfd254140167f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.2 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 20.2 | 4 | 4 | [run](https://argusic.com/run/ad655d85-859e-494f-899c-cd164b6f3652) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler (golang.org) not found in container`
- `config/app.go missing (only app.go.backup present)`
- 1 min: `Package resolution failed: go_movies/config not found under GOROOT`
- 3 min: `Redis not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
