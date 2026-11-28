# podcast-maker

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FelippeChemello/podcast-maker, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/podcast-maker

## Pinned environment

- Project commit: `5975680155af52a5b22cf3a5d07c4fbc313ce55d`
- Test commit: `5975680155af52a5b22cf3a5d07c4fbc313ce55d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 7.2 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3 | 7.2 | 2 | 2 | [run](https://argusic.com/run/c5021fbc-a6d4-42d7-b1c3-162c3f85250d) |
| 2 | pass with mocks | 92 | 10 | 8.9 | 6 | 6 | [run](https://argusic.com/run/4eabf21a-26d1-42a5-bd51-7f7c0c055054) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `ERR_PNPM_IGNORED_BUILDS on first pnpm install - core-js, esbuild, puppeteer, yarn build scripts blocked`
- `Azure TTS, Google API, YouTube credentials not configured`

Attempt 2:

- 1 min: `pnpm not installed in container`
- 2 min: `ERR_PNPM_IGNORED_BUILDS - pnpm 12 blocks build scripts by default`
- 2 min: `Content template creates width=0 and height=0, causing Remotion validation error`
- 1 min: `staticFile('') causes 404 when audioFilePath is empty`
- 1 min: `Segment model uses 'word' field not 'text'`
- 3 min: `YoutubeWrapper interpolate inputRange [0,30,80,230,280,durationInFrames] fails when durationInFrames < 280 inside shorter Sequence`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
