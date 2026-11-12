# Maintainerr

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Maintainerr/Maintainerr, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/maintainerr

## Pinned environment

- Project commit: `ed16d22b37aca3349e4d144f4e452cec88bce79f`
- Test commit: `ed16d22b37aca3349e4d144f4e452cec88bce79f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 12.4 to 82.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 82.7 | 4 | 4 | [run](https://argusic.com/run/13ea4ae7-fcb9-4ff0-944d-ef17a66b033a) |
| 2 | pass | 100 | 12 | 12.4 | 3 | 3 | [run](https://argusic.com/run/6a0116ba-555f-41e4-a857-3a069922bd0c) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Node.js v18 installed, requires >=26.0.0`
- 2 min: `yarn not on PATH`
- `UI vitest shard 1/2: 9 tests failed out of 224 (timeout flakes in TestMediaItem and RuleCreator specs)`
- `Server jest shard 2/3: 2 email notification spec failures (HTML rendering line-break comparison)`

Attempt 2:

- 2 min: `Node.js version is 18 not the required 26`
- 1 min: `corepack not bundled with Node 26 binary's npm (no corepack command)`
- 0.5 min: `data/ directory missing - project needs it for SQLite database`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
