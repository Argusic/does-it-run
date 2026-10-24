# ResumeForge

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/magicapple123/ResumeForge, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/resumeforge

## Pinned environment

- Project commit: `27c14a6e1c68c60f721f0b8bc0f45e93e5e537e6`
- Test commit: `27c14a6e1c68c60f721f0b8bc0f45e93e5e537e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.7 to 25.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 25.7 | 2 | 2 | [run](https://argusic.com/run/5177102e-de33-474e-88e4-f52676987d4c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js v18.19.1 too old for vite 8.x (requires >=20.19.0)`
- 1 min: `Missing Chinese font for server-side PDF export`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
