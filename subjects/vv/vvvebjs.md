# VvvebJs

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/givanz/VvvebJs, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/vvvebjs

## Pinned environment

- Project commit: `1acbab7ebfe3e7b004f1f18c039d26550fc04bd8`
- Test commit: `1acbab7ebfe3e7b004f1f18c039d26550fc04bd8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 4 | 0 | 0 | [run](https://argusic.com/run/e69bea1d-1226-4159-b1f1-45054e857efb) |
| 2 | pass | 100 | 7.3 | 8 | 2 | 2 | [run](https://argusic.com/run/4d930135-5635-44b4-ad3a-fbbdf0dc7bcf) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Submodule demo/landing directory was empty (not checked out)`
- `node-sass compiled for Node NODE_MODULE_VERSION 108 but system has 109, breaking gulp SCSS compilation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
