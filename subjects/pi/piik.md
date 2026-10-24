# Piik

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TNTcraftHIM/Piik, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/piik

## Pinned environment

- Project commit: `bd59e7f798835dec3f2964a9d3688096df45c37d`
- Test commit: `bd59e7f798835dec3f2964a9d3688096df45c37d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.2 | 3 | 3 | [run](https://argusic.com/run/55cbde01-1432-4d89-8e2e-41348217ad4d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 installed but v24.19.0 required (>=24.0.0 <27)`
- 2 min: `Go compiler not found, required for server binary`
- 3 min: `zip/unzip commands not installed, causing test failure: spawnSync zip ENOENT`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
