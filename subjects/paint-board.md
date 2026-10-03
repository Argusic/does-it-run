# paint-board

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LHRUN/paint-board, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/paint-board

## Pinned environment

- Project commit: `57265d7458fcfe04a0a85e3acf6745a176e0baf6`
- Test commit: `57265d7458fcfe04a0a85e3acf6745a176e0baf6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22 to 22 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29 | 22 | 4 | 4 | [run](https://argusic.com/run/c97467ec-7538-4d72-b60c-29fdc799a085) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm not available in container`
- 1 min: `pnpm blocked build scripts (canvas, esbuild, onnxruntime-node, protobufjs, sharp) due to supply-chain security policy`
- 4 min: `Native canvas module (node-canvas v2.11.2) failed to compile , missing pixman-1 dev headers (libpixman-1-0 runtime is installed but no .pc or headers)`
- 8 min: `vite-plugin-pwa 0.20.5 failed during build: Dynamic require of workbox-build not supported (and even after updating to 1.3.0, workbox-build 7.4.1 crashed with 'crypto is not defined')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
