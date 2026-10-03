# xodus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JetBrains/xodus, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/xodus

## Pinned environment

- Project commit: `18f573765aff1bf12f45f73224ae3ec7e95268e3`
- Test commit: `18f573765aff1bf12f45f73224ae3ec7e95268e3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.6 to 14.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 14.7 | 1 | 1 | [run](https://argusic.com/run/3025ebd4-66d4-4584-8b7f-c5933aa79d03) |
| 2 | pass | 100 | 7 | 12.6 | 1 | 1 | [run](https://argusic.com/run/8c88b640-7b94-46af-a85a-fdd868e26a84) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No JDK installed in container`

Attempt 2:

- 1 min: `No JDK found in container (Java not installed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
