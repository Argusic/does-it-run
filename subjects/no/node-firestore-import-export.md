# node-firestore-import-export

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jloosli/node-firestore-import-export, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/node-firestore-import-export

## Pinned environment

- Project commit: `58db1841731d99ea95255e3f05be28f0a8daa0c7`
- Test commit: `58db1841731d99ea95255e3f05be28f0a8daa0c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.4 to 26.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 26.4 | 2 | 2 | [run](https://argusic.com/run/b96de935-6cad-4ca9-aca0-f4a405d230e2) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `npm install's prepare script failed: 'snyk protect' returned 'Authentication failed. Please check the API token on https://snyk.io'`
- 8 min: `Firestore emulator would not start: Java not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
