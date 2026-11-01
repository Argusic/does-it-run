# axios

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/axios/axios, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/axios

## Pinned environment

- Project commit: `961241f6c19798eff16b0869486c125430a17961`
- Test commit: `961241f6c19798eff16b0869486c125430a17961`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 6.3 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.3 | 2 | 2 | [run](https://argusic.com/run/9bf16b93-2981-4c05-8bc7-d6a417d53c36) |
| 2 | pass with mocks | 92 | 0.5 | 7 | 1 | 1 | [run](https://argusic.com/run/e6fcbca8-69a4-4136-b8da-9603839c9e9c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 too old for vitest/rolldown (requires node:util.styleText, native bindings)`
- 1 min: `Missing @rolldown/binding-linux-x64-gnu native binding (ignore-scripts=true prevents optional dep install)`

Attempt 2:

- 5 min: `vitest 4.x test runner requires Node >=20 for its vite/rolldown dependencies (uses node:util.styleText and node:util.parseEnv which don't exist in Node 18)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
