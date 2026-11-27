# riff

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rootscripts/riff, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/riff

## Pinned environment

- Project commit: `bd725edeb4686a37f307ddd3a75da1ebcb8b07d6`
- Test commit: `bd725edeb4686a37f307ddd3a75da1ebcb8b07d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21.3 to 21.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 21.3 | 7 | 7 | [run](https://argusic.com/run/67d74cb8-403c-47b6-a0c5-793ea057751c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing root-level shim modules for test require() resolution (server, track-sort, lyrics-rtl)`
- 1 min: `stopServer() not defined or exported in server`
- 1 min: `tests read ../app.js but it only exists under src/renderer/`
- 1 min: `test vm.runInNewContext missed the second IIFE (fetch patching)`
- 1 min: `spotify auth test safeStorage mock missing getSelectedStorageBackend`
- 1 min: `require cache clearing didn't clear underlying server module state`
- 1 min: `track-sort module missing title-asc/artist-asc/duration-asc sort modes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
