# ponzu

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ponzu-cms/ponzu, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/ponzu

## Pinned environment

- Project commit: `5c57b559e76bbde372cfe2551caca252f3633abf`
- Test commit: `5c57b559e76bbde372cfe2551caca252f3633abf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.9 to 16.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 16.9 | 3 | 3 | [run](https://argusic.com/run/b5ef02f9-491f-4360-a46d-4f2d6e3a7236) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go (1.22+) not installed`
- 3 min: `GOPATH-mode go get failed on modern Go; no go.mod found`
- 3 min: `golang.org/x/crypto v0.57.0 requires go 1.26+; building with go 1.22.10`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
