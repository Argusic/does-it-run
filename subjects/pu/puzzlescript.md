# PuzzleScript

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/increpare/PuzzleScript, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/puzzlescript

## Pinned environment

- Project commit: `d236596d993b6ebb7988f1a078f582c0840ccbca`
- Test commit: `d236596d993b6ebb7988f1a078f582c0840ccbca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.6 to 11.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 11.6 | 2 | 2 | [run](https://argusic.com/run/d6223642-af8a-409e-afb8-4c5364ab28d8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `gifsicle@7 is ESM-only, cannot require() it from CJS compile.js`
- 3 min: `compress-images internally require('gifsicle') also fails with ESM error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
