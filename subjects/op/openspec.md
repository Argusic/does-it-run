# OpenSpec

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Fission-AI/OpenSpec, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openspec

## Pinned environment

- Project commit: `2500d6da971336167548b53731a35b2127df35ac`
- Test commit: `2500d6da971336167548b53731a35b2127df35ac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 86.6 to 86.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 86.6 | 1 | 1 | [run](https://argusic.com/run/9bbd1bf2-a5cd-4a17-b767-aa0e91c6c7c4) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 is below the required >=20.19.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
