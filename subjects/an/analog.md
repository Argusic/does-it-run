# analog

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/analogjs/analog, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/analog

## Pinned environment

- Project commit: `0a15065658e7f90aec71ca688b4530765b3f90dd`
- Test commit: `0a15065658e7f90aec71ca688b4530765b3f90dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 84.9 to 84.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 84.9 | 5 | 5 | [run](https://argusic.com/run/10d7236e-d3b1-4651-b544-6d6e759089c7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not pre-installed (required pnpm v11+)`
- 2 min: `Node.js v18 too old (required ^22.22.3 || ^24.15.0)`
- 5 min: `Build failed: native bindings not found for 7 apps (installed under Node 18, running on Node 22)`
- 2 min: `Test failures: Playwright browser not installed`
- 2 min: `Test failures in platform:typed-routes-consumer spec timed out at 5s default`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
