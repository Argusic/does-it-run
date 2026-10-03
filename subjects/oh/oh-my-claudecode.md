# oh-my-claudecode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Yeachan-Heo/oh-my-claudecode, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/oh-my-claudecode

## Pinned environment

- Project commit: `aaf38829060979006d37018c1648fe17b7b9918e`
- Test commit: `aaf38829060979006d37018c1648fe17b7b9918e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 30.5 to 59.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 59.2 | 4 | 4 | [run](https://argusic.com/run/71ee6a16-ccc2-472f-a117-024bcd891f18) |
| 2 | pass | 100 | 3.2 | 51 | 3 | 3 | [run](https://argusic.com/run/54e3a542-fc3f-4828-bcd4-175c6534f654) |
| 3 | pass | 100 | 3 | 30.5 | 4 | 4 | [run](https://argusic.com/run/dde4d076-a2b8-49cf-9637-c9db012c3e9e) |

## What was observed on a clean machine

Attempt 1:

- `Node.js v18.19.1 installed but project requires 20+ (engine warning from npm install)`
- `ESM entrypoint dist/index.js uses 'import ... with { type: 'json' }' which fails on Node 18`
- `Tests: installer-plugin-agents, installer-version-guard, shared-state-locking fail on Node 18`
- `npm-package-bin-surface.test.ts and plugin-shipping-surface.test.ts hang (likely npm pack with Node 18)`

Attempt 2:

- 2.2 min: `rename over non-empty dir returns EEXIST on Node 22 instead of ENOTEMPTY`
- `inventory baseline drift: 3 lint tests fail because generated manifest != expected baseline`
- `bridge-routing test times out on vitest worker pool in this env`

Attempt 3:

- `Node 18.19.1 below engine requirement (20.x || 22.x || 23.x || 24.x || 25.x || 26.x)`
- `better-sqlite3 lockfloor lint test fails on Node 18 (engine not in supported set)`
- `inventory-graph provenance test fails: ISSUE_3702_HEAD not ancestor of shallow checkout HEAD`
- `inventory-graph verify mode fails on shallow checkout`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
