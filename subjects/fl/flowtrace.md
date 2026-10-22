# Flowtrace

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AIScientists-Dev/Flowtrace, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/flowtrace

## Pinned environment

- Project commit: `1571c76365c02c13d50b943cedd36e3b21865757`
- Test commit: `1571c76365c02c13d50b943cedd36e3b21865757`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 7.8 | 1 | 1 | [run](https://argusic.com/run/eb1c344d-a9d2-44de-8d37-d1843f4e6616) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Frontend build failed: @tailwindcss/oxide missing native binding on Node 18 (npm's optional dependencies bug)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
