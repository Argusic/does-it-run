# rebrowser-patches

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rebrowser/rebrowser-patches, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/rebrowser-patches

## Pinned environment

- Project commit: `b5cb2266ec062d2797ecf081d6a3f6073feceac0`
- Test commit: `b5cb2266ec062d2797ecf081d6a3f6073feceac0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 2.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 2.4 | 0 | 0 | [run](https://argusic.com/run/b4edb4bb-c054-4cab-88f1-2a08152d9bc2) |
| 2 | pass | 100 | 8 | 8.4 | 3 | 3 | [run](https://argusic.com/run/88b79a01-3d55-4784-843b-13381b0b2273) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js v18.19.1 below required >= 22`
- 1 min: `unzip binary missing, @puppeteer/browsers extraction failed`
- 0.5 min: `Incomplete chrome install from prior failed attempt blocked reinstall`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
