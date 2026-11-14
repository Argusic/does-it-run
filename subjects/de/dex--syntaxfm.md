# dex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/syntaxfm/dex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/66511b2a-b27a-480c-90aa-ca835ac83e74

## Pinned environment

- Project commit: `3f55b2a3ec9746fc56cf62037ca6a828555ce17d`
- Test commit: `3f55b2a3ec9746fc56cf62037ca6a828555ce17d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3 to 3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.1 | 3 | 1 | 1 | [run](https://argusic.com/run/66511b2a-b27a-480c-90aa-ca835ac83e74) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Array.prototype.toSorted is not available in Node.js 18 (project requires >=24.0.0). Used in 3 source files via 'tasks.toSorted(...)' calls.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
