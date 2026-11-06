# trafilatura

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/adbar/trafilatura, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/trafilatura

## Pinned environment

- Project commit: `c852cae9708a59f04521b19395d8ed49771a5c78`
- Test commit: `c852cae9708a59f04521b19395d8ed49771a5c78`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.1 to 36.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.7 | 6.1 | 1 | 1 | [run](https://argusic.com/run/eac99dbc-f187-496b-a64e-d21ec98e6b8c) |
| 2 | pass | 100 | 0.22 | 36.4 | 4 | 4 | [run](https://argusic.com/run/6a4a262e-029a-456c-803b-5a8826cc4e73) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `trafilatura CLI binary not on PATH when tests ran subprocess(['trafilatura', '--help'])`

Attempt 2:

- 0.1 min: `pip install failed: externally-managed-environment (PEP 668)`
- 0.02 min: `test_climain: subprocess could not find 'trafilatura' binary on PATH`
- 0.02 min: `test_cli_pipeline: list-process.txt used httpbin.org URLs not covered by the mock network fixture`
- 0.01 min: `test_input_filtering: assert on httpbin.org URL count failed after list-process.txt changed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
