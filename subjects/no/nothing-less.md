# nothing-less

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mpryor/nothing-less, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/nothing-less

## Pinned environment

- Project commit: `aa9901f6df9f6f116584a31a44961cf6482b4d3f`
- Test commit: `aa9901f6df9f6f116584a31a44961cf6482b4d3f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.2 to 11.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.2 | 11.2 | 3 | 3 | [run](https://argusic.com/run/77ba7233-63d9-4851-b09c-1e872efb2bf6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Python 3.12 installed but project requires 3.13+`
- 1 min: `zoneinfo database missing US/* timezones (US/Eastern, US/Pacific) , 2 test failures in test_type_detection.py`
- `1 perf test (stream_sort_100k) slightly over threshold: 4.396s vs 4.20s limit , minor timing regression on constrained hw`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
