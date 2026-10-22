# dsh-desktop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dataelement/dsh-desktop, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dsh-desktop

## Pinned environment

- Project commit: `87df2859444d4f62ff3ac2de89a633719c788cc3`
- Test commit: `87df2859444d4f62ff3ac2de89a633719c788cc3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 30.6 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/ac5327ff-ba53-45c2-ba32-2e673f38f3ef) |
| 2 | pass | 100 | 27 | 30.6 | 4 | 4 | [run](https://argusic.com/run/49cbb36e-2929-49a4-bebe-c3bd91e0623a) |

## What was observed on a clean machine

Attempt 2:

- 10 min: `Office runtime preparation fails on Linux (unsupported platform linux/x64) - scripts/office-runtime/prepare.mjs throws`
- 1 min: `Electron sandbox fails in container without CAP_SYS_ADMIN`
- 2 min: `Node.js v18 (system) is too old; project requires Node 22+`
- `26 tests fail on Linux - all related to unsupported Linux platform (Office/Python runtime, Harness native subprocess, font rendering)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
