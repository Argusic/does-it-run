# sealeap-amazon-skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xjli360/sealeap-amazon-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/sealeap-amazon-skills

## Pinned environment

- Project commit: `497d4b8eebb484edbcdb481143a88392e963612b`
- Test commit: `497d4b8eebb484edbcdb481143a88392e963612b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.7 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 4.7 | 1 | 1 | [run](https://argusic.com/run/245cbb67-141f-4a99-98f3-88b4c69fe7ae) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `jsonschema Python module not installed in container, so mcp_research.py --schema-file/--call schema validation failed ('Schema validation requires jsonschema >= 4.18')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
