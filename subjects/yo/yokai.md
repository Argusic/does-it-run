# yokai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ankorstore/yokai, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/yokai

## Pinned environment

- Project commit: `09f538c2cf979cdd1d151f1ae9feba361f028bcf`
- Test commit: `09f538c2cf979cdd1d151f1ae9feba361f028bcf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.5 to 39.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 39.5 | 5 | 5 | [run](https://argusic.com/run/14f56e0c-6e69-459f-8cf7-068b76430226) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `trace module failed to build: OTEL SDK v1.24.0 incompatible with trace v1.38.0`
- 3 min: `httpserver middleware test failure: prometheus GatherAndCompare error format changed`
- 3 min: `fxmetrics TestModule failure: go_memstats_lookups_total not emitted by Go 1.26/prometheus v1.22.0`
- 1 min: `fxorm TestModuleDecoration failure: missing fxlog dependency`
- 2 min: `fxsql auxiliary DSN not read from config, causing SQL open with format-string literal`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
