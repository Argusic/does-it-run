# pinloop-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pinloop-ai/pinloop-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pinloop-cli

## Pinned environment

- Project commit: `7707fbc42c22c5413dd50da57b2a369dbfbdeef0`
- Test commit: `7707fbc42c22c5413dd50da57b2a369dbfbdeef0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 5.9 | 2 | 2 | [run](https://argusic.com/run/78c97985-5417-4435-8986-69a93d518e17) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `container has Node.js v18; project requires >=22`
- 1 min: `mock /count API response missing 'window' field with 'kind' property, causing TypeError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
