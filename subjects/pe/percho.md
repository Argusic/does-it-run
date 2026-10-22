# percho

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jaxton07/percho, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/percho

## Pinned environment

- Project commit: `2db9bec6e4839dc71c93ff1128fd73e172d7ecb4`
- Test commit: `2db9bec6e4839dc71c93ff1128fd73e172d7ecb4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10.8 | 0 | 0 | [run](https://argusic.com/run/8cd09e71-3cd8-414d-aa79-251d6f865fd3) |
| 2 | pass | 100 | 8 | 7.8 | 3 | 3 | [run](https://argusic.com/run/e9030856-6462-4683-8c09-a78f6b0f4257) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js 18.19.1 installed but project requires >=22.19`
- 1 min: `electron-vite build OOM (JavaScript heap out of memory)`
- `Electron SUID sandbox helper not configured`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
