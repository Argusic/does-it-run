# tengine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alibaba/tengine, licensed BSD-2-Clause, written in C.

Evidence and recordings: https://argusic.com/subject/tengine

## Pinned environment

- Project commit: `f9c9f759c029dec42ad855141fa7f0c24e9a671e`
- Test commit: `f9c9f759c029dec42ad855141fa7f0c24e9a671e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.7 to 12.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.3 | 12.7 | 4 | 4 | [run](https://argusic.com/run/eddae356-fe39-4387-9fee-683dba515ee8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PCRE library not found at configure time`
- 0.5 min: `zlib library not found at configure time`
- 0.5 min: `Permission denied installing to /usr/local/tengine (no root)`
- 0.3 min: `Permission denied binding to port 80`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
