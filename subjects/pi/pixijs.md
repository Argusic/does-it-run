# pixijs

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pixijs/pixijs, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pixijs

## Pinned environment

- Project commit: `75865b2a34596a2119c1d3fc29e2f55365c371ab`
- Test commit: `75865b2a34596a2119c1d3fc29e2f55365c371ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services, no run possible
- Valid runs: 4; wall time 48 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 48 | 5 | 5 | [run](https://argusic.com/run/b71d3a0d-b65e-4ad9-8f8f-613bd26ab13c) |
| 1 | pass with mocks | 92 | 0.7 | 60.2 | 6 | 6 | [run](https://argusic.com/run/c432bd4c-2b53-4af0-b0f2-0d1b45c7e44d) |
| 2 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/513d3933-fd95-4689-833d-a3cdaeead6f4) |
| 3 | pass | 100 | 18 | 80.9 | 7 | 7 | [run](https://argusic.com/run/04f97292-ac07-4923-becb-9be23ec6fde5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18 too old for dependencies; needs Node 20+`
- 1 min: `npm engine-strict blocked install of @es-joy/jsdoccomment requiring Node 20+`
- 1 min: `Electron SUID sandbox helper not configured`
- `WebGPU tests fail - no GPU adapter in container`
- `Text metrics precision differences - font rendering differs in this container`

Attempt 1:

- 0.3 min: `Node 18.19.1 incompatible with @es-joy/jsdoccomment@0.79.0 which requires node >=20`
- 0.8 min: `Build scripts (.mts) require tsx to run - node can't import .mts directly`
- 0.3 min: `Rollup native module @rollup/rollup-linux-x64-gnu missing (npm optional deps bug)`
- 0.5 min: `Rollup config uses import ... with { type: 'json' } syntax unsupported in Node 18`
- 10 min: `jest-electron test runner fails in headless container (electron 32 requires --no-sandbox --use-gl=swiftshader; renderer window fails to load in window-pool)`
- 0.2 min: `structuredClone not available in Node 18 causing Color test failure`

Attempt 3:

- 1 min: `npm install blocked by engine-strict=true requiring Node 24+`
- 5 min: `.mts TypeScript scripts can't run on Node 18`
- 1 min: `Rollup config uses 'with { type: 'json' }' unsupported on Node 18`
- 1 min: `exports.mts requires fs-extra/esm (ESM-only) from CJS`
- 1 min: `Electron sandbox prevents test execution`
- 1 min: `GlobalSetup imports ESM-only get-port module`
- 1 min: `Tests hang in parallel with electron runner`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
