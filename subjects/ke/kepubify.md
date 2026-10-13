# kepubify

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pgaskin/kepubify, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/kepubify

## Pinned environment

- Project commit: `9546034bc023891af5ce30709de6ae2dcf264628`
- Test commit: `9546034bc023891af5ce30709de6ae2dcf264628`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.5 to 2.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 2.5 | 1 | 1 | [run](https://argusic.com/run/b94e7dca-cba4-456b-9507-38d8eb5b9f12) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Go toolchain installed in container (go not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
