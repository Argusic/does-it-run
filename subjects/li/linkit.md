# linkit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/blue-idea/linkit, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/linkit

## Pinned environment

- Project commit: `9edfebb69078c154a1306867eb0d52223e12f1ac`
- Test commit: `9edfebb69078c154a1306867eb0d52223e12f1ac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 2.2 | 1 | 1 | [run](https://argusic.com/run/67f80360-f1ca-4e4c-9533-280329822357) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Test file used import.meta.dirname which is Node 21+ only; container has Node v18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
