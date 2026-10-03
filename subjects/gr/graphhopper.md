# graphhopper

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/graphhopper/graphhopper, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/graphhopper

## Pinned environment

- Project commit: `c1a6369ee4edc87626b41a4d842ed0373af1ce66`
- Test commit: `c1a6369ee4edc87626b41a4d842ed0373af1ce66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37.1 to 37.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 37.1 | 3 | 3 | [run](https://argusic.com/run/0bc6cf38-cdf2-42c7-a9e4-01d93c7a990a) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No JDK installed, project targets Java 25`
- 1 min: `No Maven installed`
- 2 min: `Initial JDK 21 doesn't support targeting release 25`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
