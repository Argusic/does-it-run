# nopus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Vistyy/nopus, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nopus

## Pinned environment

- Project commit: `d486f32343a933c202d788c1a75c09e771d5ee94`
- Test commit: `d486f32343a933c202d788c1a75c09e771d5ee94`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 2.8 | 1 | 1 | [run](https://argusic.com/run/461169d8-29ef-4de0-84d9-cce04283d87b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18 is installed but the project requires >=22. Also pnpm v9 is installed but the project specifies pnpm@11.21.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
