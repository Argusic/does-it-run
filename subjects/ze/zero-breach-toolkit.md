# Zero-Breach-Toolkit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/interplains/Zero-Breach-Toolkit, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/zero-breach-toolkit

## Pinned environment

- Project commit: `465134c6795302f95f66a1f80204f583ab328ca0`
- Test commit: `465134c6795302f95f66a1f80204f583ab328ca0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2 to 69.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 69.9 | 1 | 1 | [run](https://argusic.com/run/f4e8c1c4-2ee7-4c8a-9ef8-3a6f6ab425ac) |
| 2 | pass | 100 | 1 | 2 | 0 | 0 | [run](https://argusic.com/run/52f1f90f-5c9e-4440-a480-ae6d1251ee3d) |

## What was observed on a clean machine

Attempt 1:

- 0.25 min: `Missing optional cryptography dependency for encrypted iOS backup tests (84 tests skipped initially)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
