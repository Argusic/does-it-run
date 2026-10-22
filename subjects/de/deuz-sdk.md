# Deuz-SDK

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Deuz-AI/Deuz-SDK, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/deuz-sdk

## Pinned environment

- Project commit: `66040db585bd0bf0ae16842c83e56526ecfbaec4`
- Test commit: `66040db585bd0bf0ae16842c83e56526ecfbaec4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.9 to 59 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 59 | 0 | 0 | [run](https://argusic.com/run/79e40c76-49c0-4771-81d7-594df4276800) |
| 2 | pass | 100 | 5 | 6.9 | 2 | 2 | [run](https://argusic.com/run/6e4a87ae-d1a1-4ee3-ba0b-f4a6ecc396e7) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `System Node.js v18.19.1 is too old (project requires >=22)`
- 1 min: `npm install --ignore-scripts worker OOM during tsup build due to ~1GB memory limit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
