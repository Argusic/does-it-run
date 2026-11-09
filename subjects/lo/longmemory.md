# LongMemory

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CaviraOSS/LongMemory, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/longmemory

## Pinned environment

- Project commit: `9ee2c8e1ed42d83eb788afb9ffc3a82b84405da5`
- Test commit: `9ee2c8e1ed42d83eb788afb9ffc3a82b84405da5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.5 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 8.9 | 0 | 0 | [run](https://argusic.com/run/9f65b8eb-9abc-4ea7-926c-459303c11bdd) |
| 2 | pass | 100 | 5 | 4.5 | 3 | 3 | [run](https://argusic.com/run/3bdbb26c-0e45-4268-91f0-a3bffdcb0936) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `System Node.js is v18.19.1 but project requires >=20`
- `better-sqlite3 install script errored on node_gyp_bins lstat after successfully building the .node binary`
- `keytar native build failed: missing libsecret-1-dev system library`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
