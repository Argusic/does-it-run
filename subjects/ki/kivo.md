# Kivo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TrisH0x2A/Kivo, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/kivo

## Pinned environment

- Project commit: `5a6efe4189cedf0b2be52672d92f368b6223997f`
- Test commit: `5a6efe4189cedf0b2be52672d92f368b6223997f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.4 | 3 | 3 | [run](https://argusic.com/run/cabf0450-30ab-4d68-9e2b-568d1f074b70) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `contract-validation.js uses crypto.randomUUID() without importing node:crypto on Node 18`
- 1 min: `workspace-store.js uses crypto.randomUUID() without importing node:crypto on Node 18`
- 1 min: `Vite 7 requires Node 22+ (crypto.hash) but container has Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
