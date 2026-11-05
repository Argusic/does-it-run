# lemo-opuscar

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lemomo-ai/lemo-opuscar, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/lemo-opuscar

## Pinned environment

- Project commit: `e3cb16f63768c68693ff0e15171d6e755457cc32`
- Test commit: `e3cb16f63768c68693ff0e15171d6e755457cc32`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.1 to 31.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.75 | 31.7 | 1 | 1 | [run](https://argusic.com/run/7bca3a12-abf7-40ea-96f3-b6ecc050f254) |
| 2 | pass | 100 | 2 | 7.1 | 5 | 5 | [run](https://argusic.com/run/cc224e78-6815-4cdd-a442-0cb69db06fca) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `System Node.js is v18.19.1, project requires >=20. npm install fails without upgrade.`

Attempt 2:

- 2 min: `Standard installer failed because Node 18.19.1 was rejected by Playwright, which requires Node 20 or newer.`
- 1 min: `Direct rendering of styles/art-deco/demo failed with a 404 for Limelight-Regular.ttf and the page error 'A network error occurred.'`
- 1 min: `The smoke fixture initially failed readcheck because five labels were shown for only 1.20 seconds each.`
- 4 min: `mux.sh falsely rejected a valid 6.000-second WAV, reporting only 3.1 seconds decoded because FFmpeg 6.1 loudnorm progress timestamps ended early.`
- `The container lacked /usr/bin/time.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
