# analog

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/analogjs/analog, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/analog

## Pinned environment

- Project commit: `0a15065658e7f90aec71ca688b4530765b3f90dd`
- Test commit: `0a15065658e7f90aec71ca688b4530765b3f90dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 49.3 to 84.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 84.9 | 5 | 5 | [run](https://argusic.com/run/10d7236e-d3b1-4651-b544-6d6e759089c7) |
| 2 | pass | 95 | 2.5 | 49.3 | 4 | 3 | [run](https://argusic.com/run/3ab2e487-0e29-4282-841c-a4186dfca63d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not pre-installed (required pnpm v11+)`
- 2 min: `Node.js v18 too old (required ^22.22.3 || ^24.15.0)`
- 5 min: `Build failed: native bindings not found for 7 apps (installed under Node 18, running on Node 22)`
- 2 min: `Test failures: Playwright browser not installed`
- 2 min: `Test failures in platform:typed-routes-consumer spec timed out at 5s default`

Attempt 2:

- 0.5 min: `pnpm not found in container`
- 1 min: `Node.js 18 too old (project requires ^22.22.3 || ^24.15.0)`
- 1 min: `Missing @rolldown/binding-linux-x64-gnu (optional dep not installed)`
- `2 test suites have pre-existing 5s timeout flakiness in this container (router:test, platform:test)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
