# kitsu

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wopian/kitsu, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kitsu

## Pinned environment

- Project commit: `1ab8739506fe6f7aafc6543dfb2a44e6fb9e2071`
- Test commit: `1ab8739506fe6f7aafc6543dfb2a44e6fb9e2071`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.2 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 8.2 | 4 | 4 | [run](https://argusic.com/run/991609bc-ef36-4d47-96dd-30a461718091) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `yarn lockfile resolves size-limit@12.1.0 which requires Node 20+ but only Node 18 available`
- 0.7 min: `Build failure: import attribute 'with { type: 'json' }' syntax unsupported by Node 18`
- 0.5 min: `docs:typescript fails with TS5112 on TypeScript 6.0.3 (flags changed)`
- 0.8 min: `Built CJS output named .js in "type":"module" package; require('kitsu') fails per README promise`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
