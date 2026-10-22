# MxPage

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ziguishian/MxPage, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mxpage

## Pinned environment

- Project commit: `7adb826dbd8b2119222f3e3daee09a251c2fd476`
- Test commit: `7adb826dbd8b2119222f3e3daee09a251c2fd476`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28.2 to 28.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 43 | 28.2 | 4 | 4 | [run](https://argusic.com/run/8ab739f6-fa23-4156-b7b5-11c791860011) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `node:sqlite not in Node 18; custom migration script and tests require it`
- 5 min: `sharp could not load on Node 18 (requires >=20.9.0)`
- 3 min: `@modelcontextprotocol/client missing transitive dependency`
- 3 min: `npm run prisma:deploy uses custom script requiring node:sqlite but runs under system Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
