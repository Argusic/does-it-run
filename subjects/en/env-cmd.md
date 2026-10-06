# env-cmd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/toddbluhm/env-cmd, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/env-cmd

## Pinned environment

- Project commit: `18eada77f67dcd63089195992dc059f2b65c9bf1`
- Test commit: `18eada77f67dcd63089195992dc059f2b65c9bf1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.95 | 6.7 | 1 | 1 | [run](https://argusic.com/run/b137761e-ce3b-4a0e-a8c8-869d02834dc4) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Pre-built dist/parse-args.js uses Node 21+ import assertion syntax 'with { type: json }', failing on Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
