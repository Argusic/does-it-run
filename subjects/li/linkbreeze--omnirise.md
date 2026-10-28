# LinkBreeze

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OmniRise/LinkBreeze, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/8dcc61ea-33ef-4756-a8df-1cdfbab7cdf2

## Pinned environment

- Project commit: `c41555abc47fe3cf90e1164d7316b2feb7c67f86`
- Test commit: `c41555abc47fe3cf90e1164d7316b2feb7c67f86`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31 to 31 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 31 | 5 | 5 | [run](https://argusic.com/run/8dcc61ea-33ef-4756-a8df-1cdfbab7cdf2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container had Node.js v18 but project requires >=22`
- 1 min: `npm ci left rolldown native binding missing (optional dependency issue on non-x64 host check)`
- 1 min: `Domains test failed: 'no such table: domains' , DB migrations not applied`
- 2 min: `Backup-store test failure: prior test created a current-timestamp backup that sorted before test fixtures`
- 5 min: `next build repeatedly OOM'd during type-checking`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
