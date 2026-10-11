# camera.ui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cameraui/camera.ui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/camera-ui

## Pinned environment

- Project commit: `c5fcc086058848de14b1040ca068f9874a1583df`
- Test commit: `c5fcc086058848de14b1040ca068f9874a1583df`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.1 to 13.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 45 | 13.1 | 3 | 3 | [run](https://argusic.com/run/1b9dcc9b-4ec8-46b7-b150-9b3bd09dc15b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 too old (requires >=22.18.0)`
- 2 min: `UI build OOM during vue-tsc type-check (max-old-space-size default too low)`
- 1 min: `Missing config directory on first server launch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
