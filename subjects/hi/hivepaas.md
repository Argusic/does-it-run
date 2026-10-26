# hivepaas

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hivepaas/hivepaas, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/hivepaas

## Pinned environment

- Project commit: `f7185c3117195f620b28b54cfc2b3321ab7243c0`
- Test commit: `f7185c3117195f620b28b54cfc2b3321ab7243c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.2 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 12.2 | 1 | 1 | [run](https://argusic.com/run/8b172875-5ab2-4c35-a215-2681a05e6596) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `lz4 and zstd CLI binaries missing from PATH, causing 36 compress/decompress tests to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
