# goplantuml

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jfeliu007/goplantuml, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/goplantuml

## Pinned environment

- Project commit: `81d136b30c93094a3a54e46940f9e9ef3bf0ee18`
- Test commit: `81d136b30c93094a3a54e46940f9e9ef3bf0ee18`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 3.9 | 1 | 1 | [run](https://argusic.com/run/1b5b7729-f8ca-480d-a325-fcbd62b9cae9) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go toolchain not installed in container (no go binary found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
