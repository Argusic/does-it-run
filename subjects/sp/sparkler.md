# sparkler

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chrismattmann/sparkler, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/sparkler

## Pinned environment

- Project commit: `2a27562d1a99d6f7fe8c8893a1c344c3e8c76900`
- Test commit: `2a27562d1a99d6f7fe8c8893a1c344c3e8c76900`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.1 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 7.1 | 5 | 5 | [run](https://argusic.com/run/2e212f8c-1e62-4294-96c0-b8a9923a7786) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Java 21 not installed on container`
- 1 min: `Node 18 (v18.19.1) too old for Vite 8 rolldown native bindings`
- 0.5 min: `Rolldown native binding missing after Node upgrade`
- 1 min: `Solr process killed when shell session ended`
- `sparkler solr status fails without lsof`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
