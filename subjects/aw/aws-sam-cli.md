# aws-sam-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aws/aws-sam-cli, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/aws-sam-cli

## Pinned environment

- Project commit: `3a8d3c2d0b7e4d618e51239b3f4fa4ee405d2c4f`
- Test commit: `3a8d3c2d0b7e4d618e51239b3f4fa4ee405d2c4f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.9 to 11.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.9 | 1 | 1 | [run](https://argusic.com/run/14fe025c-72e7-405c-bc3b-49d03ed94564) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_updates_imageuri_when_pointing_to_local_archive wrote to path escaping /work/repo (PermissionError)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
