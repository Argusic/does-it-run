# AlgerMusicPlayer

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/algerkong/AlgerMusicPlayer, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/algermusicplayer

## Pinned environment

- Project commit: `0e056506a2f0744ed5664e6de46a3433fa835cda`
- Test commit: `0e056506a2f0744ed5664e6de46a3433fa835cda`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 8.8 to 17.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 8.8 | 5 | 5 | [run](https://argusic.com/run/49755599-8b84-421d-81b7-8fe2f77dcd39) |
| 2 | pass | 100 | 17 | 17.3 | 2 | 2 | [run](https://argusic.com/run/a2d98b3c-ca3c-494c-aba9-3ed505ee6e54) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm postinstall: electron-builder install-app-deps failed on Node 18 (abstract-socket native rebuild)`
- 2 min: `downloadMetadata.test.ts: ESM-only music-metadata@12 causes SyntaxError on Node 18`
- 1 min: `playbackController.test.ts: CustomEvent not defined in Node 18`
- `electron-vite build fails on Node 18 ESM resolution bug`
- `Electron sandbox requires sudo for chrome-sandbox`

Attempt 2:

- 2 min: `CustomEvent not defined in Node 18 (playbackController tests)`
- 3 min: `music-metadata/file-type uses Node 20+ /v regex flag (downloadMetadata test suite crash)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
