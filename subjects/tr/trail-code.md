# Trail-Code

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/trailhq/Trail-Code, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/trail-code

## Pinned environment

- Project commit: `8dc7a63b26dc1b8137bacc33390b6ed6279c1212`
- Test commit: `8dc7a63b26dc1b8137bacc33390b6ed6279c1212`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 86.6 to 86.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 86.6 | 3 | 3 | [run](https://argusic.com/run/ca111e71-0d8e-404d-af22-9d08529d252c) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `npm test failed 1 subtest: "a process killed while holding the lock releases it" (test/graph-refresh.test.ts) , the spawned 'node -e' child died with SyntaxError "await is only valid in async functions" on Node 18, which runs -e as CommonJS`
- 12 min: `The full test suite never printed while run through 'npm test' redirected to a file in this shell because the runner's buffered output stayed empty and a child from test/viz-serve.test.ts wedged in ep_poll for ~22 minutes (an environment qu`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
