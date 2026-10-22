# CodeAF

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Agent-Field/CodeAF, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/codeaf

## Pinned environment

- Project commit: `794b49a57894655bd129a15a24b519d0f7b8d5c8`
- Test commit: `794b49a57894655bd129a15a24b519d0f7b8d5c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 30.5 to 30.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26.8 | 30.5 | 3 | 3 | [run](https://argusic.com/run/9bcc555a-4827-4292-8677-a464af34f688) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `go toolchain not installed: Go 1.26.5+ required but no go binary on PATH`
- 1 min: `make build fails with '/bin/sh: 1: Bad substitution' on plandb CGO link step`
- `make size and test targets print '/bin/sh: 1: Bad substitution' at end even after SHELL fix (from CGO subprocess invoking /bin/sh directly)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
