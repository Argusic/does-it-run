# Nora

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Sandakan/Nora, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nora

## Pinned environment

- Project commit: `5c2b5ab3767e886d9cbce0d15a4a2c5673a1c7e8`
- Test commit: `5c2b5ab3767e886d9cbce0d15a4a2c5673a1c7e8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4.5 | 2 | 2 | [run](https://argusic.com/run/57cf6f70-0cbd-49fb-b77a-b43672f28a36) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18.19.1 too old , requires ^20.19.0 || >=22.12.0`
- 1 min: `npm v10.9.9 too old , requires ^11.6.2`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
