# reader

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vakra-dev/reader, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/reader

## Pinned environment

- Project commit: `df1a48b57e5d540bed801f0d9bbeaee9168eb2cd`
- Test commit: `df1a48b57e5d540bed801f0d9bbeaee9168eb2cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.6 to 12.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 12.5 | 4 | 4 | [run](https://argusic.com/run/1e457761-5760-4933-8a2a-ae9d387d57b8) |
| 2 | pass with mocks | 92 | 4.5 | 3.6 | 2 | 2 | [run](https://argusic.com/run/14b76140-2cbc-4b23-b693-8027b4b0d418) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 too old for vitest v4 (needs node:util.styleText)`
- 2 min: `Missing @rolldown/binding-linux-x64-gnu native binary (installed from npm under Node 18)`
- 8 min: `Daemon failed to launch Chrome (spawn google-chrome ENOENT)`
- 3 min: `playwright-core bundled into dist by tsup, causing runtime require failure`

Attempt 2:

- 3 min: `Node.js v18 (container default) is too old for vitest 4.1.0 and rolldown native bindings , 'styleText' missing in node:util, and binding-linux-x64-gnu not found`
- 0.5 min: `npm prefix config in project .npmrc conflicted with npm link`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
