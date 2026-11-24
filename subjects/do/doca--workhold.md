# doca

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/workhold/doca, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/f45a32e8-8dad-49dd-ad81-984aa93820b0

## Pinned environment

- Project commit: `e7cd975189dd894e31a5beb136a5040dbaed1ce0`
- Test commit: `e7cd975189dd894e31a5beb136a5040dbaed1ce0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 35.7 to 85.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 79 | 85.8 | 1 | 1 | [run](https://argusic.com/run/f45a32e8-8dad-49dd-ad81-984aa93820b0) |
| 2 | pass | 80 | 36 | 35.7 | 3 | 0 | [run](https://argusic.com/run/68bd64e9-7bfd-422f-9980-2ae07dcf2fdf) |

## What was observed on a clean machine

Attempt 1:

- 45 min: `better-sqlite3@13.0.3 prebuilt native modules (prebuilds/linux-x64.node) require node_register_module_v127 which Node.js v22+ does not export dynamically, causing SIGSEGV on load`

Attempt 2:

- `92 tests fail with trusted_engine_required (no Python ML/SAM2 engine)`
- `5 AI tests timed out`
- `20 AI tests need real model responses (image gen, doc parsing, canvas vision)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
