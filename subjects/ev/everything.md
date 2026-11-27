# everything

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HeyPuter/everything, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/everything

## Pinned environment

- Project commit: `a7f61cdc2eee2957f579b242c0d4f4fe3331ce9c`
- Test commit: `a7f61cdc2eee2957f579b242c0d4f4fe3331ce9c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.3 to 3.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.3 | 1 | 1 | [run](https://argusic.com/run/367793a2-0dde-4769-a12a-4e87591932bb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18.19.1 too old for Vite 8.x/vitest 4.x dependencies (rolldown needs node:util.styleText)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
