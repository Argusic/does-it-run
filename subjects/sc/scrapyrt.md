# scrapyrt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/scrapinghub/scrapyrt, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/scrapyrt

## Pinned environment

- Project commit: `6d00a0ad55c310c268fb13a151a3f3c98f0cabb4`
- Test commit: `6d00a0ad55c310c268fb13a151a3f3c98f0cabb4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 5.2 | 1 | 1 | [run](https://argusic.com/run/428e255f-96d4-41db-8813-4a63996360c4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `flask command not found on PATH when running integration tests (Flask installed only in venv)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
