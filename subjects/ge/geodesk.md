# geodesk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/clarisma/geodesk, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/geodesk

## Pinned environment

- Project commit: `5215f8c48a1faabcbc4254c90b634988dd5a7a14`
- Test commit: `5215f8c48a1faabcbc4254c90b634988dd5a7a14`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.9 | 2 | 2 | [run](https://argusic.com/run/fc734314-37f8-4a3e-a941-b9b8f57c2444) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No JDK or Maven in the container`
- 1 min: `Apache download site returned 404 for Maven binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
