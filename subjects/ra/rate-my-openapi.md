# rate-my-openapi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zuplo/rate-my-openapi, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/rate-my-openapi

## Pinned environment

- Project commit: `24819fbe7576e2811b3be2750312e2cea64bcf14`
- Test commit: `24819fbe7576e2811b3be2750312e2cea64bcf14`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.1 | 7.2 | 2 | 2 | [run](https://argusic.com/run/3fa81c2c-b62c-49f2-9b02-4d627fa4775d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `vacuum CLI not on PATH when invoked by internal-cli generate-rating`
- 5 min: `@tailwindcss/oxide native binding not found , Node 18 vs required >=20`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
