# goneovim

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/akiyosi/goneovim, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/goneovim

## Pinned environment

- Project commit: `d6d80cc8d1783ee4f08242892c483f16fe9aff90`
- Test commit: `d6d80cc8d1783ee4f08242892c483f16fe9aff90`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 70.7 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/25c96565-bb26-47a3-b6f2-163c223cdbbd) |
| 2 | pass with mocks | 92 | 30 | 70.7 | 5 | 5 | [run](https://argusic.com/run/84727109-16c8-4f8d-92a9-e3f8fec955aa) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Go 1.22.2 not installed`
- 10 min: `Qt5 system packages not installed (no root access)`
- 10 min: `Qt5 CGo compilation fails cascade of missing headers`
- 3 min: `Qt5 runtime libraries missing for linker`
- `Test segfaults on stub Qt objects at runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
