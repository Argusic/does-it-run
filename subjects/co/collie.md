# collie

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AltanS/collie, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/collie

## Pinned environment

- Project commit: `2bec9cbd64118561b58eddf1701371dc95e831ea`
- Test commit: `2bec9cbd64118561b58eddf1701371dc95e831ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 12.3 | 2 | 2 | [run](https://argusic.com/run/590e432f-e9ba-4964-ae41-e5272e326a02) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Bun not found in container`
- 2 min: `Node.js 18 too old for Vite 8.x (needs 20.19+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
