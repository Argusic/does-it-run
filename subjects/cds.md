# cds

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ovh/cds, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/cds

## Pinned environment

- Project commit: `efa68e88c86a1dc90f9b0fe4f941ffe6775e2368`
- Test commit: `efa68e88c86a1dc90f9b0fe4f941ffe6775e2368`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 42.3 to 42.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 42.3 | 4 | 4 | [run](https://argusic.com/run/59fcd7a5-4086-42c8-9905-a2db037daddb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Go toolchain in container`
- 2 min: `No PostgreSQL available`
- 1 min: `No Redis available`
- 1 min: `SQL migrations failed on PG 9.3 (no jsonb type)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
