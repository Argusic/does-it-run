# sveltepress

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SveltePress/sveltepress, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/sveltepress

## Pinned environment

- Project commit: `f3ab25be2d823463335d698a7f14136ea4c97089`
- Test commit: `f3ab25be2d823463335d698a7f14136ea4c97089`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12 to 12 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 12 | 3 | 3 | [run](https://argusic.com/run/c108229d-ed31-414a-aaa1-61ff523ea10a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18.19.1 is below project minimum (^20.19.0 or >=22.12.0)`
- 1 min: `pnpm not found in environment`
- `packages/vite prepare script (unbuild) hit V8 heap OOM (Reached heap limit Allocation failed - JavaScript heap out of memory)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
