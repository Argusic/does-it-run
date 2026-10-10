# grafbase

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/grafbase/grafbase, licensed MPL-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/grafbase

## Pinned environment

- Project commit: `b8223903090f38b50d74c6678656d90d4e8dadb7`
- Test commit: `b8223903090f38b50d74c6678656d90d4e8dadb7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 63.9 to 63.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 63.9 | 3 | 3 | [run](https://argusic.com/run/a9f4eae7-338c-4199-aa1d-b711ad12ba63) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Rust toolchain not installed`
- 0.3 min: `CLI build script panic: missing assets/cli-app.tar.gz`
- `Integration tests failed: 19 failures in graphql_over_http, subscriptions, mtls`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
