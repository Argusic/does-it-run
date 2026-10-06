# eva.js

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eva-engine/eva.js, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/eva-js

## Pinned environment

- Project commit: `792ede99108c5af56ff724c2e136747406895d02`
- Test commit: `792ede99108c5af56ff724c2e136747406895d02`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.8 to 24.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.37 | 24.8 | 6 | 6 | [run](https://argusic.com/run/cdd68e7a-81a3-4478-be9a-1671c080650d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `jest.config.js mapped @eva/inspector-decorator to non-existent path /work/inspector-decorators/src`
- 1 min: `mesh.spec.ts expected component.resource === undefined but default is empty string`
- 1 min: `decorators.spec.ts expected size field isArray=false, actual returns isArray=true, addable=true`
- 3 min: `resource.spec.ts expected PixiJS Warning from mock pixi.js that never emits it; listening/error tests timeout`
- 2 min: `matterjs.spec.ts TS error: sides not on Body type`
- 1 min: `rollup.config.js mapped @eva/inspector-decorator to non-existent path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
