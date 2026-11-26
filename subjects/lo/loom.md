# loom

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ClickHouse/loom, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/loom

## Pinned environment

- Project commit: `2b9544afb03cb34d027893307283793570ec413c`
- Test commit: `2b9544afb03cb34d027893307283793570ec413c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 69.2 to 69.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 69.2 | 3 | 3 | [run](https://argusic.com/run/1cf73139-75b9-4ac7-8471-54676d95f253) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing numpy dependency for conflict resolver module`
- 1 min: `Missing tree-sitter/tree-sitter-typescript for code parser tests`
- 1 min: `Missing schemathesis for contract tests (optional extra)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
