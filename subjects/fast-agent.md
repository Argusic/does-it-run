# fast-agent

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/evalstate/fast-agent, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/fast-agent

## Pinned environment

- Project commit: `920cb671f3478cc54ea4c5ac993a3d923750d135`
- Test commit: `920cb671f3478cc54ea4c5ac993a3d923750d135`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 19.4 to 30.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 19.4 | 0 | 0 | [run](https://argusic.com/run/93653658-ade5-468a-bab1-2f70a1377419) |
| 2 | pass | 100 | 0.15 | 30.2 | 2 | 2 | [run](https://argusic.com/run/ce15db30-6af2-4c1e-9582-9529a05ab44d) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `test_cli_duckdb_sql_rejects_multiple_statements_before_execution failed: _normalize_user_sql() ran after _parquet_view_query(), so a missing-file IOError masked the SQL validation`
- 3 min: `test_prefixed_method_signatures_wrap_to_documented_width failed: inspect.Signature.format(max_width=...) is Python 3.13+ only, project targets 3.12`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
