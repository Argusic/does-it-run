# doca

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/workhold/doca, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/f45a32e8-8dad-49dd-ad81-984aa93820b0

## Pinned environment

- Project commit: `e7cd975189dd894e31a5beb136a5040dbaed1ce0`
- Test commit: `e7cd975189dd894e31a5beb136a5040dbaed1ce0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 85.8 to 85.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 79 | 85.8 | 1 | 1 | [run](https://argusic.com/run/f45a32e8-8dad-49dd-ad81-984aa93820b0) |

## What was observed on a clean machine

Attempt 1:

- 45 min: `better-sqlite3@13.0.3 prebuilt native modules (prebuilds/linux-x64.node) require node_register_module_v127 which Node.js v22+ does not export dynamically, causing SIGSEGV on load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
