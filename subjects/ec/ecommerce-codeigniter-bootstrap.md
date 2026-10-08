# Ecommerce-CodeIgniter-Bootstrap

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kirilkirkov/Ecommerce-CodeIgniter-Bootstrap, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/ecommerce-codeigniter-bootstrap

## Pinned environment

- Project commit: `911626df1d3204c9a5f09d120f338987bb0927ee`
- Test commit: `911626df1d3204c9a5f09d120f338987bb0927ee`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.2 to 18.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 18.2 | 6 | 6 | [run](https://argusic.com/run/5f5aa31e-bd26-4e6e-b4a0-3a86a01a8bc4) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP 8.3 not installed in container`
- 3 min: `MariaDB not installed in container`
- 2 min: `PHP mysqli extension not loaded`
- 1 min: `ctype extension missing (ctype_digit undefined)`
- 2 min: `mbstring extension missing (mb_strtoupper undefined)`
- 2 min: `MariaDB port mismatch (installer uses default 3306, server started on 3307)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
