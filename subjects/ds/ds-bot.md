# DS-Bot

**Verdict: runs with mocks.** Argusic Score 85.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Fei2411/DS-Bot, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ds-bot

## Pinned environment

- Project commit: `de55888a93983fc51c94f7d22bc94b4f8293205d`
- Test commit: `de55888a93983fc51c94f7d22bc94b4f8293205d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.5 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 85.33 | 3 | 5.5 | 3 | 2 | [run](https://argusic.com/run/cb5a365b-e34d-4f8b-b7ab-a7c6075bcdd5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 installed but project requires v22.19+`
- `app/package-lock.json out of sync (missing ws@8.22.0), npm ci failed`
- `App test fails: ws@8.22.0 is a peer dependency not listed in 'dependencies'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
