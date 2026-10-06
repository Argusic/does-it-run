# read-aloud

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ken107/read-aloud, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/read-aloud

## Pinned environment

- Project commit: `b590ee60a6fb80c0446597dac924d755823bca95`
- Test commit: `b590ee60a6fb80c0446597dac924d755823bca95`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 5.5 to 10.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 5 | 10.4 | 1 | 1 | [run](https://argusic.com/run/6c7a50a5-64a8-41d2-9310-0affba557754) |
| 2 | pass | 100 | 0.5 | 5.5 | 2 | 2 | [run](https://argusic.com/run/6d8763ea-ac66-4ce8-acb4-6d6ba945cf8a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm run package failed: 'zip' command not found`

Attempt 2:

- 1 min: `npm run package failed: zip command not found`
- 1 min: `playwright latest (1.63) requires node>=20, container has node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
