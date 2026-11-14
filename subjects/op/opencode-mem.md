# opencode-mem

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tickernelz/opencode-mem, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opencode-mem

## Pinned environment

- Project commit: `a2072d75eaecf9998f1e93ac68bc1a38dfd1db33`
- Test commit: `a2072d75eaecf9998f1e93ac68bc1a38dfd1db33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 8.9 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.1 | 12.6 | 1 | 1 | [run](https://argusic.com/run/fa071492-03fc-4cd7-a34c-a31f09172d5c) |
| 2 | pass | 100 | 14 | 8.9 | 2 | 2 | [run](https://argusic.com/run/3e3c5dba-4d5a-45bd-b562-bc717f2379c3) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `web:build failed on system Node 18 , svelte-check/vite require Node >=20 or Bun's runtime`

Attempt 2:

- 4 min: `Missing @img/sharp-linux-x64 native binary (sharp optional dep) caused onnxruntime-resolve test to fail with 'Could not load sharp module'`
- 2 min: `Missing dist/ directory caused 13 plugin-loader-contract/bundle-boundary tests to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
