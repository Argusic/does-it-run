# vaultite

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Vaultite/vaultite, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vaultite

## Pinned environment

- Project commit: `03e06df12e8cd1e0711eef82e788a4f56746bc4d`
- Test commit: `03e06df12e8cd1e0711eef82e788a4f56746bc4d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 13.1 to 18.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 18.6 | 0 | 0 | [run](https://argusic.com/run/b41c72a7-085a-4d27-b0b7-8529b8f94498) |
| 2 | pass | 100 | 1.5 | 13.1 | 3 | 3 | [run](https://argusic.com/run/4bb2ed91-c5e1-4c86-99d3-ba7ca3a4f929) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js v18.19.1 installed but project requires >=23.6 , import.meta.dirname and Type Stripping missing`
- 0.3 min: `.npmrc had ignore-scripts=true and min-release-age=7 which blocked native binary rebuilds (esbuild, node-pty) and package resolution`
- 1 min: `process.threadCpuUsage is not a function , crashes in saves, share, cotype test areas`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
