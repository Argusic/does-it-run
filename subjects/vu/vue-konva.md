# vue-konva

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/konvajs/vue-konva, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vue-konva

## Pinned environment

- Project commit: `eedf13ce9f42f62051a717428520d8771032f78b`
- Test commit: `eedf13ce9f42f62051a717428520d8771032f78b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 5.2 | 3 | 3 | [run](https://argusic.com/run/87f207f4-837e-4403-8b20-fe97a591a065) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Container has Node 18.19.1 but the project's devDependencies (vite 8.2.2, vitest 4.1.11, jsdom 30) require Node >=22 (vite: ^20.19||>=22.12, vitest: ^20||^22, jsdom: ^22.22.2). npm test crashed at startup: 'node:util' does not provide 'styl`
- 3 min: `Rolldown's native binding was not installed (npm optional-dependencies bug, npm/cli#4828): 'Cannot find native binding ... @rolldown/binding-wasm32-wasi'.`
- 2 min: `Running tests on Node 20 failed with 'webidl.util.markAsUncloneable is not a function' because jsdom 30 pulls undici 8 which needs Node >=22.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
