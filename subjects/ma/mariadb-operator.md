# mariadb-operator

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mariadb-operator/mariadb-operator, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/mariadb-operator

## Pinned environment

- Project commit: `b04f95f3af57b8e076948f637186683efb09c7ed`
- Test commit: `b04f95f3af57b8e076948f637186683efb09c7ed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 38.6 to 38.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 38.6 | 4 | 4 | [run](https://argusic.com/run/c01715d9-ed58-4820-8db3-d05d7e6ad713) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go 1.27.2 not found in PATH (required by go.mod)`
- 3 min: `Helm not found (needed by helm chart unit tests)`
- 2 min: `make test-api + test-pkg + test-helm partly failed initially because helm chart dependencies were missing`
- 12 min: `make test-webhook fails with 'too many open files' (0x18) on BeforeSuite when a prior webhook test run's etcd process is left alive`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
