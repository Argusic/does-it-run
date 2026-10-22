# Restfox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/flawiddsouza/Restfox, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/restfox

## Pinned environment

- Project commit: `74ba395f84993297146e70805e2cc1c6a03f21c7`
- Test commit: `74ba395f84993297146e70805e2cc1c6a03f21c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4 | 3 | 3 | [run](https://argusic.com/run/000af871-c1cf-4254-9e38-8e5e92412f63) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `vite build: fatal: No names found, cannot describe anything`
- 1.5 min: `ReferenceError: File is not defined in undici with Node 18.19.1`
- 1 min: `TypeError: Cannot read properties of undefined in undici decompress with Node 22.14.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
