# anti-slop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dmmulroy/anti-slop, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/ccb75d1a-803f-48c2-a5ae-4a56d0ac30f1

## Pinned environment

- Project commit: `c44ef22ca116d0ba62a3ff663a0bd13a3f3fa40b`
- Test commit: `c44ef22ca116d0ba62a3ff663a0bd13a3f3fa40b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.5 to 12.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 12.5 | 3 | 3 | [run](https://argusic.com/run/ccb75d1a-803f-48c2-a5ae-4a56d0ac30f1) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm not found in container`
- 0.2 min: `oxlint native binding @oxlint/binding-linux-x64-gnu missing (optional dependency not installed by default)`
- 3 min: `Node.js 18 lacks import.meta.dirname support and cannot load .ts plugin files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
