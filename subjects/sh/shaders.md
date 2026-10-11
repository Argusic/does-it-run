# shaders

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shader-effects-inc/shaders, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/shaders

## Pinned environment

- Project commit: `81fd4ece5d493ca6c424a2af41f0e2c361ec8258`
- Test commit: `81fd4ece5d493ca6c424a2af41f0e2c361ec8258`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 10.2 | 3 | 3 | [run](https://argusic.com/run/922eea37-696e-468f-8aff-ce21b01421e4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Preinstalled Node 18 without pnpm; repo requires Node 22.20.x and pnpm 10.0.0`
- 2 min: `pnpm warned 'build scripts ignored' for esbuild, sharp, svelte-preprocess, vue-demi because package.json pnpm.onlyBuiltDependencies was []`
- 3 min: `WebGPU rendering cannot run in this container (no GPU/WebGPU device); renderer degrades gracefully by design and GPU-free tests pass`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
