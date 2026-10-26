# acryl

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/acryldev/acryl, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/acryl

## Pinned environment

- Project commit: `686f9fa7efda21dd2c4efe13746aa11e2918db7e`
- Test commit: `686f9fa7efda21dd2c4efe13746aa11e2918db7e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.7 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 13.7 | 2 | 2 | [run](https://argusic.com/run/36234310-e2e0-49fc-ad0b-092d66f20c50) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.19.1 installed but project requires ^22.19.0 or >=24.0.0`
- `Surface-parity test: 2 Loader rows only Web composes (allowlist gap)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
