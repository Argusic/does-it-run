# video-react

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/video-react/video-react, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/video-react

## Pinned environment

- Project commit: `d6718bc69f8dfd2306a17424151128ea6bc57afa`
- Test commit: `d6718bc69f8dfd2306a17424151128ea6bc57afa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.3 to 1.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.12 | 1.3 | 1 | 1 | [run](https://argusic.com/run/99221af2-0caa-492b-b314-3dc39472d80f) |
| 2 | pass | 100 | 2 | 1.7 | 1 | 1 | [run](https://argusic.com/run/6219611a-2ff4-466c-a5f7-10e437bd89f5) |

## What was observed on a clean machine

Attempt 1:

- `Rollup build fails: @rollup/plugin-terser requires Node >=20 (current: 18.19.1)`

Attempt 2:

- `npm run build fails: Rollup plugin-terser crashes with 'crypto is not defined' in serialize-javascript on Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
