# vhs

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/charmbracelet/vhs, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/vhs

## Pinned environment

- Project commit: `c073383b5de0b1f57bf514113029c306bc986539`
- Test commit: `c073383b5de0b1f57bf514113029c306bc986539`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 16.4 to 51.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 24.8 | 2 | 2 | [run](https://argusic.com/run/21a70ca6-d6bb-4909-9fda-800512393e3b) |
| 2 | pass | 100 | 50 | 51.4 | 5 | 5 | [run](https://argusic.com/run/60440855-e514-4eb0-a49c-cb2f2ef7abc0) |
| 3 | pass | 100 | 14 | 16.4 | 4 | 4 | [run](https://argusic.com/run/7df745c0-5953-4996-988a-cc323e1182a6) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `VHS binary created GIF output file but frames directory remained empty - canvas elements not found in xterm.js used by ttyd 1.7.7`
- 8 min: `GIF output not created despite 'Creating simple.gif...' log message and exit code 0`

Attempt 2:

- 2 min: `go not installed`
- 1 min: `ttyd not installed`
- 1 min: `Chromium sandbox killed browser (no --no-sandbox)`
- 2 min: `evaluator called v.Render(ctx) after teardown() cancelled ctx, killing ffmpeg before it could run`

Attempt 3:

- 2 min: `Go not installed in container`
- 1 min: `ttyd not installed`
- 1 min: `Chrome sandbox crash: 'No usable sandbox!' in container`
- 5 min: `GIF output never written (ffmpeg killed by cancelled context)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
