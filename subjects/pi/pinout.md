# pinout

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/j0ono0/pinout, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pinout

## Pinned environment

- Project commit: `d46f4f1949b1360a07bc52a04c32f786975d702c`
- Test commit: `d46f4f1949b1360a07bc52a04c32f786975d702c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34.7 to 34.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 34.7 | 4 | 4 | [run](https://argusic.com/run/0e04475b-56fc-477a-a238-d62884c2c452) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `CWD not restored on exception in export_diagram() caused cascade test failures`
- 3 min: `Floating-point precision differences between Python versions caused SVG content mismatches in tests`
- 1 min: `Windows backslash path separators in reference SVGs made them mismatch Linux-generated output`
- 1 min: `Missing Python packages: pandas, openpyxl, libsass needed by sample diagram scripts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
