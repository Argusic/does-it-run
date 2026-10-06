# pr-lens

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coldteadotai/pr-lens, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pr-lens

## Pinned environment

- Project commit: `1b597ef8ad756c25d78ec5b51553db47935ff95b`
- Test commit: `1b597ef8ad756c25d78ec5b51553db47935ff95b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.8 | 1 | 1 | [run](https://argusic.com/run/45a44d6b-18bf-4b52-9b32-5b907571c3da) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 in environment does not satisfy engine requirement >=20.11 (and vite needs ^20.19.0 or >=22.12.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
