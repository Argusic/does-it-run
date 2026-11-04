# mycli

**Verdict: runs.** Argusic Score 84 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dbcli/mycli, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/mycli

## Pinned environment

- Project commit: `709272fadf5d6d8c293601b03df38c3dc5af8169`
- Test commit: `709272fadf5d6d8c293601b03df38c3dc5af8169`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 5.9 to 19.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 19.8 | 4 | 4 | [run](https://argusic.com/run/609c79e9-be6c-473b-a6e2-ee3b9aeeff03) |
| 2 | fail | 68 | 2 | 5.9 | 5 | 2 | [run](https://argusic.com/run/7e68fd05-e20b-41d7-a5e3-160c12ece948) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not pre-installed in container`
- 1 min: `test.utils import path not in sys.path for standalone pytest`
- 10 min: `MariaDB 13.0.2 binary crashes intermittently between shell sessions in this container`
- `5 pytest failures against MariaDB due to MySQL/MariaDB compatibility (SSL, EXPLAIN, error messages)`

Attempt 2:

- 1 min: `uv package manager not found in container PATH`
- 0.5 min: `Initial pytest run failed on polars/altair/llm tests due to missing optional dependencies`
- `79 pytest tests skipped (dbtest marker) requiring a MySQL server; 0 installed and no root access`
- `Behave integration tests (8 features, 43 scenarios) cannot run without a MySQL server`
- `External tools less, fzf, pygmentize missing from container; runtime-only, not required for test suite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
