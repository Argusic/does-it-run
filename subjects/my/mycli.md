# mycli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dbcli/mycli, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/mycli

## Pinned environment

- Project commit: `709272fadf5d6d8c293601b03df38c3dc5af8169`
- Test commit: `709272fadf5d6d8c293601b03df38c3dc5af8169`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.8 to 19.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 19.8 | 4 | 4 | [run](https://argusic.com/run/609c79e9-be6c-473b-a6e2-ee3b9aeeff03) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not pre-installed in container`
- 1 min: `test.utils import path not in sys.path for standalone pytest`
- 10 min: `MariaDB 13.0.2 binary crashes intermittently between shell sessions in this container`
- `5 pytest failures against MariaDB due to MySQL/MariaDB compatibility (SSL, EXPLAIN, error messages)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
