# loop-engineering

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cobusgreyling/loop-engineering, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/loop-engineering

## Pinned environment

- Project commit: `7422449e2297736eebd48e9600e604cb2f71cc3b`
- Test commit: `7422449e2297736eebd48e9600e604cb2f71cc3b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.7 to 27.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 27.6 | 3 | 3 | [run](https://argusic.com/run/a6e4fa6b-c718-4fde-ab98-57c5afb37169) |
| 2 | pass | 100 | 8 | 9.7 | 2 | 2 | [run](https://argusic.com/run/803aac94-d591-49f7-b4fd-a8a54f10cd16) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `loop-audit failing 2 tests , ERR_MODULE_NOT_FOUND for readiness-core`
- 4 min: `loop-sandbox uses '^1.3.0' registry semver instead of local file: dependency on loop-worktree, breaking loop-swarm transitive resolution`
- 1 min: `loop-metrics test had hardcoded date 2026-07-30 that fell outside 30-day window`

Attempt 2:

- 3 min: `loop-audit clean install contained readiness-core without dist/index.js, so TypeScript could not resolve @cobusgreyling/readiness-core and the build failed.`
- 2 min: `npm ci in tools/mcp-server failed with ENOENT because npm 9 tried to materialize readiness-core inside the linked loop-audit dependency, but the lockfile had no entry for it.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
