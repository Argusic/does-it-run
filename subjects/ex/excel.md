# excel

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nusr/excel, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/excel

## Pinned environment

- Project commit: `0a7763aa39b42a0dbe06e1413b3beebfac54cb4c`
- Test commit: `0a7763aa39b42a0dbe06e1413b3beebfac54cb4c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.4 to 11.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 11.4 | 4 | 4 | [run](https://argusic.com/run/b4bb9dc7-133f-4cce-a789-9bc384f0393b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `yarn install triggers postinstall script that runs lerna build with Node 20+ features`
- 2 min: `lerna CLI uses import.meta.filename (undefined in Node 18) and require() of ES module`
- `vite 8.3.0 requires Node ^20.19.0 || >=22.12.0 , server/build unavailable on Node 18`
- `demo/backend requires @y/y peer dependency for websocket , cannot launch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
