# nsq

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nsqio/nsq, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/nsq

## Pinned environment

- Project commit: `85cf10c09c6c3c86160d6f0eb156f62d0efc1648`
- Test commit: `85cf10c09c6c3c86160d6f0eb156f62d0efc1648`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.3 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.3 | 2 | 2 | [run](https://argusic.com/run/657ab80b-6783-4903-92e2-72b34e285593) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go binary not found in PATH`
- 2 min: `Go 1.25.0 had Swiss-map internal redeclaration compiler errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
