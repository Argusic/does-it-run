# ai-gateway

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ferro-labs/ai-gateway, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/ai-gateway

## Pinned environment

- Project commit: `d025ca1a3c6e0c6a83ed7c93147e36f39a1e6cb4`
- Test commit: `d025ca1a3c6e0c6a83ed7c93147e36f39a1e6cb4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 10.1 | 3 | 3 | [run](https://argusic.com/run/f020f5b0-13ac-4c5e-a876-5660849573ea) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25.14 compiler not found in PATH`
- 1 min: `'go: cannot find GOROOT directory: go binary is trimmed and GOROOT is not set' then 'package X is not in std' errors , only the binary was copied without its stdlib src/ tree`
- 1 min: `Hundreds of 'GOPROXY list is not the empty string, but contains no entries' errors treated as build failures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
