# lunarr-go

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lunarr-app/lunarr-go, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/lunarr-go

## Pinned environment

- Project commit: `af35226b6a86b9cda3faf75e7a26b49147ed2ed0`
- Test commit: `af35226b6a86b9cda3faf75e7a26b49147ed2ed0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 7.2 | 3 | 3 | [run](https://argusic.com/run/06b14411-fdfc-4d23-8dd7-edb55078bfd5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Bun not installed in container`
- 1 min: `Node.js 18 lacks styleText export from node:util needed by rolldown`
- `bun not on PATH for npm test script`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
