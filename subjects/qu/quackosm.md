# quackosm

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kraina-ai/quackosm, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/quackosm

## Pinned environment

- Project commit: `d19b963205c5557f76a8ca271cacfcaa94fd4972`
- Test commit: `d19b963205c5557f76a8ca271cacfcaa94fd4972`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 69.5 to 69.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 1.5 | 69.5 | 2 | 1 | [run](https://argusic.com/run/ce704848-ee8f-4ff9-91c7-006880e782f8) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `cgroup memory limit 8 GB too low for DuckDB COPY with 747+ columns when keep_all_tags=True and explode_tags=True`
- 8 min: `test_displaying_osm_extracts assertion fails because Rich tree rendering wraps long extract names onto continuation lines that lack any source name prefix`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
