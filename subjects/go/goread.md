# goread

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Ray-D-Song/goread, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/goread

## Pinned environment

- Project commit: `7c25bdbb120d12176f7456973c5ebf5896c94e1a`
- Test commit: `7c25bdbb120d12176f7456973c5ebf5896c94e1a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 3.2 | 1 | 1 | [run](https://argusic.com/run/c4f666d2-ce9d-4268-b7aa-c8017d464721) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `fmt.Println with raw string literal has redundant trailing newline in cmd/goread/utils.go:82`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
