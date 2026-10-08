# bitECS

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NateTheGreatt/bitECS, licensed MPL-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/bitecs

## Pinned environment

- Project commit: `1585cdb4ae9a6586aef5e4d9d30d7039e22cd543`
- Test commit: `1585cdb4ae9a6586aef5e4d9d30d7039e22cd543`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 2.9 | 3 | 3 | [run](https://argusic.com/run/be22319f-bd36-497f-ab4f-18c268eab238) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `bun not found globally , package.json test script uses 'bun test'`
- 0.1 min: `tsc not found , build:types script calls tsc`
- 0.1 min: `tsc 7.x removed downlevelIteration and baseUrl options , tsconfig uses both`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
