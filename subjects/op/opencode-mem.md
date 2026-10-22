# opencode-mem

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tickernelz/opencode-mem, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opencode-mem

## Pinned environment

- Project commit: `a2072d75eaecf9998f1e93ac68bc1a38dfd1db33`
- Test commit: `a2072d75eaecf9998f1e93ac68bc1a38dfd1db33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.6 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.1 | 12.6 | 1 | 1 | [run](https://argusic.com/run/fa071492-03fc-4cd7-a34c-a31f09172d5c) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `web:build failed on system Node 18 , svelte-check/vite require Node >=20 or Bun's runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
