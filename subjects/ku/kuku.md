# kuku

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kuku-mom/kuku, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kuku

## Pinned environment

- Project commit: `ea07b629ead912ada70442e8c87ae90359742d33`
- Test commit: `ea07b629ead912ada70442e8c87ae90359742d33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 24 to 24 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 23 | 24 | 7 | 7 | [run](https://argusic.com/run/af374870-3d1c-4580-9888-d3cf121d44f7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not pre-installed (needed node v18)`
- 2 min: `Rust not pre-installed`
- 2 min: `Go not pre-installed`
- 2 min: `Node v18 too old for vitest 4.x (needs node:util.styleText)`
- `kuku-ai linking fails on Linux: no WebKit/GTK2/JavaScriptCore system libraries`
- `Go server tests need PostgreSQL`
- `libglib2.0-dev not installed (only runtime libs present)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
