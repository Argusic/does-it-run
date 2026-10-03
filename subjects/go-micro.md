# go-micro

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/micro/go-micro, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/go-micro

## Pinned environment

- Project commit: `3791c5ec341eb2fda61637947a50e55b71bdd662`
- Test commit: `3791c5ec341eb2fda61637947a50e55b71bdd662`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31.1 to 31.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 25 | 31.1 | 2 | 0 | [run](https://argusic.com/run/21a8a449-e013-4a89-bf69-9c8f1f51ce30) |

## What was observed on a clean machine

Attempt 1:

- `config/source/cli: test flag parsing conflict with -test.count (pre-existing, not caused by changes)`
- `internal/harness/provider-conformance: missing .github/workflows/harness.yml CI config file (pre-existing)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
