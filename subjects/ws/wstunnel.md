# wstunnel

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/erebe/wstunnel, licensed BSD-3-Clause, written in Rust.

Evidence and recordings: https://argusic.com/subject/wstunnel

## Pinned environment

- Project commit: `5b17615dda10d4635d1c415f527e7f788c08724f`
- Test commit: `5b17615dda10d4635d1c415f527e7f788c08724f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.7 to 19.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 14.7 | 3 | 3 | [run](https://argusic.com/run/d70f1339-0a3b-4e53-902c-4a927c1c2906) |
| 2 | pass | 100 | 19 | 19.9 | 2 | 2 | [run](https://argusic.com/run/0a9801fc-3f81-44ca-9089-293eead91bee) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `IPv6 disabled in container; UDP test hardcoded [::1] addresses failed (os error 99)`
- 3 min: `NO_COLOR=1 env var caused clap bool parse failure ('invalid value 1 for --no-color')`
- 1 min: `TCP proxy test uses Docker via testcontainers; no Docker in container`

Attempt 2:

- 8 min: `IPv6 is disabled at kernel level (read-only sysctl), UDP server tests bind to ::1 (IPv6 localhost) and panic`
- 5 min: `Docker is not available in the container, TCP test test_proxy_connection panics on testcontainers Docker init`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
